[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /proposals/resources

**Description**: Retrieves a list of proposal resource assignment rows with nested project and non-project work maps.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/proposals/resources`
- `url`: String, `https://<domain>/api/snapshot/proposals/resources`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Notes**:

- Response includes only resources assigned to `project_type = "proposal"` proposals.
- Response returns one object per proposal resource assignment.
- Legacy top-level period keys are still returned as a mirror of `project_work` for backward compatibility.
- Legacy top-level period keys are deprecated and scheduled for removal after `July 18, 2026`.
- `project_work` contains assignment estimates by period.
- `non_project_work` contains non-project time values for the same assignment period window.
- When the assignment has periods, `non_project_work` uses the same period keys as `project_work`, even when all values are `0`.
- For monthly companies, period keys use the `MMM YYYY` format, for example `Jan 2024`.
- For non-monthly companies, both maps use the company period display label, for example `Quarter 1 2024`.

**Response**:

```json
[
  {
    "id": 201,
    "department": "Architecture",
    "estimate": 35,
    "end_date_planned": "2024-01-31",
    "last_updated": "2024-01-12",
    "priority": null,
    "project_name": "Proposal Phoenix",
    "resource_department": "Proposal Team",
    "resource_name": "Jane Doe",
    "resource_role": "Architect",
    "risk_score": 0,
    "start_date_planned": "2024-01-01",
    "state": "ready-for-review",
    "value_score": 0,
    "Jan 2024": 50,
    "Feb 2024": 25,
    "project_work": {
      "Jan 2024": 50,
      "Feb 2024": 25
    },
    "non_project_work": {
      "Jan 2024": 25,
      "Feb 2024": 40
    }
  }
]
```

**Field Reference**:

- `id`: Integer proposal resource assignment ID
- `department`: String or `null`
- `estimate`: Integer or `null`
- `end_date_planned`: Date or `null`
- `last_updated`: Date or `null`
- `priority`: String or `null`
- `project_name`: String
- `MMM YYYY`: Deprecated top-level period keys mirrored from `project_work`, for example `Jan 2024`. These remain available until `July 18, 2026`
- `project_work`: Object keyed by period label. Values are Integer or `null`
- `non_project_work`: Object keyed by the same period labels as `project_work` when the assignment has periods. Values are Integer
- `resource_department`: String or `null`
- `resource_name`: String or `null`
- `resource_role`: String or `null`
- `risk_score`: Integer or `null`
- `start_date_planned`: Date or `null`
- `state`: String or `null`. For proposal assignment rows this is the proposal lifecycle value, for example `draft`, `deferred`, or `ready-for-review`
- `value_score`: Integer or `null`

[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /projects/resources

**Description**: Retrieves a list of project resources.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/resources`
- `url`: String, `https://<domain>/api/snapshot/projects/resources`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
    {
        "id": "integer",
        "department": "null or string",
        "estimate": "integer",
        "end_date_planned": "date",
        "last_update": "datetime",
        "priority": "option",
        "project_name": "string",
        "resource_department": "string",
        "resource_name": "string",
        "resource_role": "string",
        "risk_score": "integer",
        "start_date_planned": "date",
        "state": "option",
        "value_score": "integer",
        "Aug 2024": "integer"
    }
 ]
}
```


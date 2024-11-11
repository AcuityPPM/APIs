[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /projects/reports

**Description**: Retrieves a list of project status reports.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/reports`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
    {
        "id": 9804,
        "accomplishments": "string",
        "budget_status": "green | yellow | red",
        "created_at": "date",
        "health_status": "green | yellow | red",
        "help_needed": "string",
        "look_ahead": "string",
        "project_id": "integer",
        "project_name": "string",
        "quality_status": "green | yellow | red",
        "schedule_status": "green | yellow | red",
        "summary": "string",
        "updated_at": "date",
        "user": "string | null",
        "user_id": "string | null"
    }
 ]
}
```

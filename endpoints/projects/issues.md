[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /projects/issues

**Description**: Retrieves a list of issues.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/issues`
- `url`: String, `https://<domain>/api/snapshot/projects/issues`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
    {
        "id": "integer",
        "action_plan": "text",
        "created_at": "date",
        "description": "text",
        "issue_owner": "string",
        "name": "string",
        "notes": "text",
        "priority": "option",
        "project_id": "integer",
        "project_name": "string",
        "resolution": "text",
        "resolution_date": "date",
        "status": "option",
        "updated_at": "date"
    }
 ]
}
```


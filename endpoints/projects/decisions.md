[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /projects/decisions

**Description**: Retrieves a list of project decisions.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/decisions`
- `url`: String, `https://<domain>/api/v1/projects/decisions`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
    {
        "id": "integer",
        "comments": "string",
        "created_at": "date",
        "decision_date": "date | null",
        "decision_marker": "string",
        "desision": "string",
        "project_id": "integer",
        "project_name": "string",
        "updated_at": "date"
    }
 ]
}
```

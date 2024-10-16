# API Endpoints

## GET /projects/decisions

**Description**: Retrieves a list of project decisions.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/image.png)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/decisions`
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

[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /projects/benefits

**Description**: Retrieves a list of project benefits.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/benefits`
- `url`: String, `https://<domain>/api/snapshot/projects/benefits`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
    {
        "id": "integer",
        "baseline_date": "date | null",
        "baseline_value": "string | null",
        "benefit_description": "string",
        "benefit_name": "string",
        "created_at": "date",
        "measurement": "string | null",
        "project_id": "integer",
        "project_name": "string",
        "status": "open | closed",
        "status_indicator": "green | yellow | red",
        "status_summary": "string | null",
        "target_date": "date | null",
        "target_value": "string | null",
        "updated_at": "date"
    }
 ]
}
```

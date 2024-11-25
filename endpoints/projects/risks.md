[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /projects/risks

**Description**: Retrieves a list of risks.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/risks`
- `url`: String, `https://<domain>/api/v1/projects/risks`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
  {
   "id": "integer",
   "created_at": "date",
   "description": "text",
   "likelihood": "option",
   "name": "string",
   "notes": "text",
   "priority": "option",
   "project_id": "integer",
   "project_name": "string",
   "response_plan": "text",
   "risk_owner": "string",
   "risk_response": "option",
   "severity": "option",
   "status": "option",
   "updated_at": "date"
   }
 ]
}
```


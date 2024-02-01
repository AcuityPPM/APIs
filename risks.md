# API Endpoints

## GET /risks

**Description**: Retrieves a list of risks.

**Example Postman**:

![Alt text](image.png)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/risks`
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

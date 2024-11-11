[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /proposals

**Description**: Retrieves a list of proposals.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/proposals`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
  {
    "id": "integer",
    "benefits": "string",
    "category": "option",
    "created_at": "date",
    "department": "option",
    "description": "text",
    "destination": "portfolio",
    "end_date": "date",
    "lifecycle": "option",
    "name": "string",
    "planned_capital_expenses": "currency",
    "planned_cost": "currency",
    "planned_operational_expenses": "currency",
    "priority": "option",
    "Custom Field name": "Custom Field value",
    "requestor": "string",
    "risk_priority_score": "integer",
    "sponsor": "string",
    "start_date": "date",
    "status": "option",
    "strategic_objective": "option",
    "value_priority_score": "integer"
  }
 ]
}
```

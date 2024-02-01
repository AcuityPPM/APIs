# API Endpoints

## GET /projects

**Description**: Retrieves a list of projects.

**Example Postman**:

![Alt text](image.png)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects`
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
    "portfolio": "portfolio",
    "end_date": "date",
    "lifecycle": "option",
    "name": "string",
    "planned_capital_expenses": "currency",
    "planned_cost": "currency",
    "planned_operational_expenses": "currency",
    "priority": "option",
    "project_custom_fields": [
        {
            "name": "Custom Field name",
            "value": "Custom Field value"
        },
    ],
    "Custom Field name": "Custom Field value",
    "requestor": "string",
    "risk_priority_score": "integer",
    "sponsor": "string",
    "start_date": "date",
    "state": "option",
    "strategic_objective": "option",
    "value_priority_score": "integer"
  }
 ]
}

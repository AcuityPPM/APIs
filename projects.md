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
    "actual_capital_expenses": "currency",
    "actual_cost": "currency",
    "actual_financial_benefits": "currency",
    "actual_operational_expenses": "currency",
    "approved_at": "date",
    "background": "string",
    "benefits": "string",
    "category": "custom option",
    "created_at": "date",
    "department": "custom option",
    "description": "text",
    "duration": "integer",
    "end_date": "date",
    "financial_class": "capital | operational",
    "funding": "planning | funded | unfunded",
    "health_status": "green | yellow | red | gray",
    "hours": "integer",
    "lifecycle": "custom option",
    "name": "string",
    "percent_complete": "0 - 100",
    "planned_capital_expenses": "currency",
    "planned_cost": "currency",
    "planned_financial_benefits": "currency",
    "planned_operational_expenses": "currency",
    "portfolio": "portfolio",
    "priority": "low | medium | high",
    "project_objectives": "string",
    "project_custom_fields": [
        {
            "name": "Custom Field name",
            "value": "Custom Field value"
        },
    ],
    "Custom Field name": "Custom Field value",
    "project_manager": "string",
    "requestor": "string",
    "risk_priority_score": "integer",
    "schedule_variance": "integer",
    "sponsor": "string",
    "start_date": "date",
    "state": "active | hold | completed | cancelled | pending",
    "strategic_objective": "custom option",
    "value_priority_score": "integer",
  }
 ]
}

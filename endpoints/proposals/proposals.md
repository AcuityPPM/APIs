[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /proposals

**Description**: Retrieves a list of proposals.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/proposals`
- `url`: String, `https://<domain>/api/snapshot/proposals`
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
    "background": "text",
    "benefits": "text",
    "category": "option",
    "closed_risks_count": "integer",
    "created_at": "date",
    "department": "option",
    "description": "text",
    "destination": "Portfolio Name",
    "end_date": "date",
    "hours": "integer",
    "lifecycle": "option",
    "name": "text",
    "open_risks_count": "integer",
    "percent_complete": "integer",
    "planned_capital_expenses": "currency",
    "planned_cost": "currency",
    "planned_financial_benefits": "currency",
    "planned_operational_expenses": "currency",
    "project_manager": "string",
    "project_objectives": "string",
    "project_token": "uuid",
    "proposal_portfolio": "string",
    "recommendations": "text",
    "requestor": "string",
    "risk_priority_score": "integer",
    "sponsor": "string",
    "start_date": "date",
    "status": "option",
    "strategic_objective": "option",
    "Business Sponsor": "string",
    "Executive Sponsor": "string",
    "IT Project Manager": "string",
    "Product Manager": "string",
    "total_risks_count": "integer",
    "value_priority_score": "integer",
    "Custom Field text": "text",
    "Custom Field integer": "integer",
    "Custom Field date": "date",
    "Custom Field currency": "currency"
  }
 ]
}
```

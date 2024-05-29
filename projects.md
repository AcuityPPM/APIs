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
    "Custom Field name": "Custom Field value",
    "actual_capital_expenses": "currency",
    "actual_cost": "currency",
    "actual_financial_benefits": "currency",
    "actual_operational_expenses": "currency",
    "approval_date": "date",
    "background": "string",
    "benefits": "string",
    "benefits_stoplight_status": "green | yellow | red | gray",
    "budget_status": "green | yellow | red | gray",
    "quality_status": "green | yellow | red | gray",
    "schedule_status": "on | ahead | behind | gray",
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
    "id": "integer",
    "last_status_report_date": "date",
    "lifecycle": "custom option",
    "name": "string",
    "percent_complete": "0 - 100",
    "planned_capital_expenses": "currency",
    "planned_cost": "currency",
    "planned_financial_benefits": "currency",
    "planned_operational_expenses": "currency",
    "portfolio": "portfolio",
    "priority": "low | medium | high",
    "project_manager": "string",
    "project_objectives": "string",
    "quality_status": "green | yellow | red | gray",
    "requestor": "string",
    "resource_stoplight_status": "green | yellow | red | gray",
    "risk_priority_score": "integer",
    "risk_stoplight_status": "green | yellow | red | gray",
    "schedule_status": "green | yellow | red | gray",
    "schedule_variance": "integer",
    "scope_stoplight_status": "green | yellow | red | gray",
    "sponsor": "string",
    "start_date": "date",
    "state": "active | hold | completed | cancelled | pending",
    "status_summary_status_report": "text",
    "accomplishments_status_report": "text",
    "help_needed_status_report": "text",
    "look_ahead_status_report": "text",
    "strategic_objective": "custom option",
    "value_priority_score": "integer",
    "Business Sponsor": "stakeholder",
    "Executive Sponsor": "stakeholder",
    "IT Project Manager": "stakeholder",
    "Product Manager": "stakeholder",
    "project_state_date": "date",
    "project_custom_fields": [
        {
            "name": "Custom Field name",
            "value": "Custom Field value"
        },
    ],
    // all custom fields with null values if no assigned to the project
    "Custom Field text": null,
    "Custom Field integer": null,
    "Custom Field date": null
  }
 ]
}

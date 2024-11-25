[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /projects

**Description**: Retrieves a list of projects.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects`
- `url`: String, `https://<domain>/api/v1/projects`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
    {
        "Custom Field name": "Custom Field value",
        "accomplishments_status_report": "text",
        "actual_capital_expenses": "currency",
        "actual_cost": "currency",
        "actual_financial_benefits": "currency",
        "actual_operational_expenses": "currency",
        "approval_date": "date",
        "background": "string",
        "benefits": "string",
        "benefits_stoplight_status": "green | yellow | red | gray",
        "budget_status": "green | yellow | red | gray",
        "category": "custom option",
        "closed_benefits_count": "integer",
        "closed_issues_count": "integer",
        "closed_risks_count": "integer",
        "created_at": "date",
        "department": "custom option",
        "description": "text",
        "duration": "integer",
        "end_date": "date",
        "financial_class": "capital | operational",
        "funding": "planning | funded | unfunded",
        "health_status": "green | yellow | red | gray",
        "help_needed_status_report": "text",
        "hours": "integer",
        "id": "integer",
        "last_status_report_date": "date",
        "last_status_report_submitted_by": "User.name | null",
        "lifecycle": "custom option",
        "look_ahead_status_report": "text",
        "name": "string",
        "open_benefits_count": "integer",
        "open_issues_count": "integer",
        "open_risks_count": "integer",
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
        "quality_status": "green | yellow | red | gray",
        "requestor": "string",
        "resource_stoplight_status": "green | yellow | red | gray",
        "risk_priority_score": "integer",
        "risk_stoplight_status": "green | yellow | red | gray",
        "schedule_status": "green | yellow | red | gray",
        "schedule_status": "on | ahead | behind | gray",
        "schedule_variance": "integer",
        "scope_stoplight_status": "green | yellow | red | gray",
        "sponsor": "string",
        "start_date": "date",
        "state": "active | hold | completed | cancelled | pending",
        "status_summary_status_report": "text",
        "strategic_objective": "custom option",
        "total_benefits_count": "integer",
        "total_issues_count": "integer",
        "total_risks_count": "integer",
        "value_priority_score": "integer",
        "Business Sponsor": "stakeholder",
        "Executive Sponsor": "stakeholder",
        "IT Project Manager": "stakeholder",
        "Product Manager": "stakeholder",
        "project_state_date": "date",
        "Custom Field text": null,
        "Custom Field integer": null,
        "Custom Field date": null
    }
 ]
}
```

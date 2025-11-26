[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/record.md)

# API Endpoints

## POST /proposal

**Description**: Create a new proposal.

**Example Postman**:

**Headers**(`domain`, `route`, `api-auth`, `api-token`, `api-secret`)

- `route`: String, `/proposal`
- `url`: String, `<domain>/api/v1/proposal`

![Headers](https://github.com/AcuityPPM/APIs/blob/main/img/post_headers.webp)
<br>
**Body**
<br>
![Body](https://github.com/AcuityPPM/APIs/blob/main/img/post_body.webp)

### Fields

**Description**: Required fields are marked with an asterisk (\*).

| Field                  | Type               | Default                     | Acuity UI Text                            |
| ---------------------- | ------------------ | --------------------------- | ----------------------------------------- |
| `proposal_portfolio`\* | `string`           | `required`                  | Proposal Portfolio Name                   |
| `name`\*               | `string`           | `required`                  | Name                                      |
| `description`\*        | `text`             | `required`                  | Description                               |
| `proposal_requestor`   | `text`             | `required`                  | Requestor                                 |
| `background`           | `text`             | `""`                        | Background                                |
| `project_type`         | `text`             | `"project"`                 | Project Type                              |
| `benefits`             | `text`             | `""`                        | Benefits                                  |
| `proposal_objectives`  | `text`             | `""`                        | Project Objectives                        |
| `recommendations`      | `text`             | `""`                        | Recommendations                           |
| `cost`                 | `integer`          | `0`                         | Total Cost (Planned)                      |
| `financial_benefits`   | `integer`          | `nil`                       | Financial Benefits (Planned)              |
| `hours`                | `integer`          | `0`                         | Total Project Hours                       |
| `percent_complete`     | `0-100`            | `0`                         | Percent Complete                          |
| `start_date`           | `date(yyyy-mm-dd)` | `nil`                       | Start Date                                |
| `end_date`             | `date(yyyy-mm-dd)` | `nil`                       | Finish Date                               |
| `category`             | `option`           | `nil`                       | Category(or your chosen name)             |
| `department`           | `option`           | `nil`                       | Department(or your chosen name)           |
| `lifecycle`            | `option`           | `nil`                       | Phase(or your chosen name)                |
| `strategic_objective`  | `option`           | `nil`                       | Strategic Objectives(or your chosen name) |
| `proposal_sponsor`     | `sponsor name`     | `nil`                       | Project Sponsor(or your chosen name)      |
| `project_manager`      | `manager name`     | `nil`                       | Project Manager(or your chosen name)      |
| `proposal_state`       | `draft`, `final`   | `"draft, ready-for-review"` | Proposal State                            |
| `priority`             | `custom option`    | `default option`            | Priorities(or your chosen name)           |

### Example of Project Custom Fields

```json
{
  "proposal_portfolio": "Proposal Portfolio",
  "name": "Proposal Name",
  "description": "Proposal Description",
  "custom_fields": {
    "Custom Text Field": "Some text",
    "Custom Integer Field": "500",
    "Custom Currency Field": "1000",
    "Custom Date Field": "2025-10-31",
    "Custom Dropdown Field": "Option 1",
    "Custom MultiSelect Field": "Option 1, Option 2"
  }
}
```

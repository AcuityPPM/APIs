[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/record.md)

# API Endpoints

## POST /project

**Description**: Create a new project.

**Example Postman**:

**Headers**(`domain`, `route`, `api-auth`, `api-token`, `api-secret`)

- `route`: String, `/project`
- `url`: String, `<domain>/api/v1/project`

![Headers](https://github.com/AcuityPPM/APIs/blob/main/img/post_headers.webp)
<br>
**Body**
<br>
![Body](https://github.com/AcuityPPM/APIs/blob/main/img/post_body.webp)

### Fields

**Description**: Required fields are marked with an asterisk (\*).

| Field                 | Type                                                  | Default          | Acuity UI Text                            |
| --------------------- | ----------------------------------------------------- | ---------------- | ----------------------------------------- |
| `portfolio`\*         | `string`                                              | `required`       | Portfolio Name                            |
| `name`\*              | `string`                                              | `required`       | Name                                      |
| `description`\*       | `text`                                                | `required`       | Description                               |
| `background`          | `text`                                                | `""`             | Background                                |
| `benefits`            | `text`                                                | `""`             | Benefits                                  |
| `project_objectives`  | `text`                                                | `""`             | Project Objectives                        |
| `cost`                | `integer`                                             | `0`              | Total Cost (Planned)                      |
| `financial_benefits`  | `integer`                                             | `nil`            | Financial Benefits (Planned)              |
| `hours`               | `integer`                                             | `0`              | Total Project Hours                       |
| `percent_complete`    | `0-100`                                               | `0`              | Percent Complete                          |
| `start_date`          | `date(yyyy-mm-dd)`                                    | `nil`            | Start Date                                |
| `end_date`            | `date(yyyy-mm-dd)`                                    | `nil`            | Finish Date                               |
| `category`            | `option`                                              | `nil`            | Category(or your chosen name)             |
| `department`          | `option`                                              | `nil`            | Department(or your chosen name)           |
| `lifecycle`           | `option`                                              | `nil`            | Phase(or your chosen name)                |
| `strategic_objective` | `option`                                              | `nil`            | Strategic Objectives(or your chosen name) |
| `project_sponsor`     | `sponsor name`                                        | `nil`            | Project Sponsor(or your chosen name)      |
| `project_manager`     | `manager name`                                        | `nil`            | Project Manager(or your chosen name)      |
| `state`               | `active`, `cancelled`, `completed`, `hold`, `pending` | `active`         | State                                     |
| `priority`            | `option`                                              | `default option` | Priorities(or your chosen name)           |
| `funding`             | `planning`, `funded`, `unfunded`                      | `nil`            | Funding Status                            |
| `financial_class`     | `capital`, `operational`                              | `nil`            | Financial Class                           |
| `team_member_1`       | `Business Sponsor name`                               | `nil`            | Business Sponsor(or your chosen name)     |
| `team_member_2`       | `Executive Sponsor name`                              | `nil`            | Executive Sponsor(or your chosen name)    |
| `team_member_3`       | `IT Project Manager`                                  | `nil`            | IT Project Manager(or your chosen name)   |
| `team_member_4`       | `Product Manager`                                     | `nil`            | Product Manager(or your chosen name)      |
| `custom_fields`       | `Object{key:value}`                                   | `nil`            | Company Custom Field                      |

### Example of Project Custom Fields

```json
{
  "portfolio": "Portfolio",
  "name": "Project Name",
  "description": "Project Description",
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

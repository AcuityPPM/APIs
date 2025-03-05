[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/record.md)

# API Endpoints

## PUT /project

**Description**: Update an existing project.

**Example Postman**:

**Headers**(`domain`, `route`, `api-auth`, `api-token`, `api-secret`)

- `route`: String, `/project`
- `url`: String, `<domain>/api/v1/project`

![Headers](https://github.com/AcuityPPM/APIs/blob/main/img/put_headers.webp)
<br>
**Body**
<br>
![Body](https://github.com/AcuityPPM/APIs/blob/main/img/put_body.webp)

### Fields

**Description**: Required fields are marked with an asterisk (\*).

| Field                 | Type                                                  | Default    | Acuity UI Text                            |
| --------------------- | ----------------------------------------------------- | ---------- | ----------------------------------------- |
| `project_token`\*     | `uuid`                                                | `required` | Project Token                             |
| `name`                | `string`                                              | `""`       | Name                                      |
| `description`         | `text`                                                | `""`       | Description                               |
| `background`          | `text`                                                | `""`       | Background                                |
| `benefits`            | `text`                                                | `""`       | Benefits                                  |
| `project_objectives`  | `text`                                                | `""`       | Project Objectives                        |
| `cost`                | `integer`                                             | `0`        | Total Cost (Planned)                      |
| `financial_benefits`  | `integer`                                             | `nil`      | Financial Benefits (Planned)              |
| `hours`               | `integer`                                             | `0`        | Total Project Hours                       |
| `percent_complete`    | `0-100`                                               | `0`        | Percent Complete                          |
| `start_date`          | `date(yyyy-mm-dd)`                                    | `nil`      | Start Date                                |
| `end_date`            | `date(yyyy-mm-dd)`                                    | `nil`      | Finish Date                               |
| `category`            | `option`                                              | `nil`      | Category(or your chosen name)             |
| `department`          | `option`                                              | `nil`      | Department(or your chosen name)           |
| `lifecycle`           | `option`                                              | `nil`      | Phase(or your chosen name)                |
| `strategic_objective` | `option`                                              | `nil`      | Strategic Objectives(or your chosen name) |
| `project_sponsor`     | `sponsor name`                                        | `nil`      | Project Sponsor(or your chosen name)      |
| `project_manager`     | `manager name`                                        | `nil`      | Project Manager(or your chosen name)      |
| `state`               | `active`, `cancelled`, `completed`, `hold`, `pending` | `active`   | State                                     |
| `priority`            | `low`, `medium`, `high`                               | `low`      | Priority                                  |
| `funding`             | `planning`, `funded`, `unfunded`                      | `nil`      | Funding Status                            |
| `financial_class`     | `capital`, `operational`                              | `nil`      | Financial Class                           |
| `custom_fields`       | `Object{key:value}`                                   | `nil`      | Company Custom Field                      |

### Example of Project Custom Fields

```json
{
  "project_token": "UUID",
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

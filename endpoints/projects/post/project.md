[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/record.md)

# API Endpoints

## POST /projects

**Description**: Create a new project.

**Example Postman**:

**Headers**(`domain`, `route`, `api-auth`, `api-token`, `api-secret`)

- `route`: String, `/projects`
- `url`: String, `<domain>/api/v1/projects`

![Headers](https://github.com/AcuityPPM/APIs/blob/main/img/post_headers.webp)
<br>
**Body**
<br>
![Body](https://github.com/AcuityPPM/APIs/blob/main/img/post_body.webp)

### Fields

**Description**: Required fields are marked with an asterisk (\*).

| Field                 | Type                                                  | Default    | Acuity UI Text                            |
| --------------------- | ----------------------------------------------------- | ---------- | ----------------------------------------- |
| `portfolio`\*         | `string`                                              | `required` | Portfolio Name                            |
| `name`\*              | `string`                                              | `required` | Name                                      |
| `description`\*       | `text`                                                | `required` | Description                               |
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

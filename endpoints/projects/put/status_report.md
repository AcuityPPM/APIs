[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## PUT /project/status-report

**Description**: Update an existing project status report.

**Example Postman**:

**Headers**(`domain`, `route`, `api-auth`, `api-token`, `api-secret`)

- `route`: String, `/project/status-report`
- `url`: String, `<domain>/api/v1/project/status-report`

![Headers](https://github.com/AcuityPPM/APIs/blob/main/img/put_headers.webp)
<br>
**Body**
<br>
![Body](https://github.com/AcuityPPM/APIs/blob/main/img/put_body.webp)

### Fields

**Description**: Required fields are marked with an asterisk (\*).

| Field                       | Type                             | Default    | Acuity UI Text   |
| --------------------------- | -------------------------------- | ---------- | ---------------- |
| `id`\*                      | `bigint`                         | `required` | Status Report ID |
| `summary`                   | `text`                           | `green`    | Summary          |
| `accomplishments`           | `text`                           | `green`    | Accomplishments  |
| `look_ahead`                | `text`                           | `green`    | Look Ahead       |
| `help_needed`               | `text`                           | `green`    | Help Needed      |
| `health_status`             | `green`, `yellow`, `red`, `gray` | `green`    | Health Status    |
| `schedule_status`           | `green`, `yellow`, `red`, `gray` | `yellow`   | Schedule Status  |
| `budget_status`             | `green`, `yellow`, `red`, `gray` | `green`    | Budget Status    |
| `quality_status`            | `green`, `yellow`, `red`, `gray` | `green`    | Quality Status   |
| `scope_stoplight_status`    | `green`, `yellow`, `red`, `gray` | `green`    | Scope Status     |
| `risk_stoplight_status`     | `green`, `yellow`, `red`, `gray` | `green`    | Risk Status      |
| `resource_stoplight_status` | `green`, `yellow`, `red`, `gray` | `green`    | Resource Status  |
| `benefits_stoplight_status` | `green`, `yellow`, `red`, `gray` | `green`    | Benefits Status  |
| `percent_complete`          | `0-100`                          | `0`        | Percent Complete |


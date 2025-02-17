[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/record.md)

# API Endpoints

## POST /project/task

**Description**: Create a new task.

**Example Postman**:

**Headers**(`domain`, `route`, `api-auth`, `api-token`, `api-secret`)

- `route`: String, `/project/task`
- `url`: String, `<domain>/api/v1/project/task`

![Headers](https://github.com/AcuityPPM/APIs/blob/main/img/post_headers.webp)
<br>
**Body**
<br>
![Body](https://github.com/AcuityPPM/APIs/blob/main/img/post_body.webp)

### Fields

**Description**: Required fields are marked with an asterisk (\*).

| Field                | Type                    | Default    | Acuity UI Text     |
| -------------------- | ----------------------- | ---------- | ------------------ |
| `project_token`\*    | `uuid`                  | `required` | Project Token      |
| `task_name`\*        | `string`                | `required` | Task Name          |
| `status`             | `open`, `closed`        | `open`     | Status             |
| `start_date`         | `date(yyyy-mm-dd)`      | `nil`      | Start Date         |
| `finish_date`        | `date(yyyy-mm-dd)`      | `nil`      | Finish Date        |
| `actual_finish_date` | `date(yyyy-mm-dd)`      | `nil`      | Actual Finish Date |
| `notes`              | `string`                | `""`       | Notes              |
| `performance`        | `green`,`yellow`, `red` | `green`    | Performance        |
| `assigned_to`        | `option`                | `nil`      | Assigned To        |

[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/record.md)

# API Endpoints

## PUT /proposal/timeline

**Description**: Update proposal dates.

**Example Postman**:

**Headers**(`domain`, `route`, `api-auth`, `api-token`, `api-secret`)

- `route`: String, `/proposal/timeline`
- `url`: String, `<domain>/api/v1/proposal/timeline`

![Headers](https://github.com/AcuityPPM/APIs/blob/main/img/post_headers.webp)
<br>
**Body**
<br>
![Body](https://github.com/AcuityPPM/APIs/blob/main/img/post_body.webp)

### Fields

**Description**: Required fields are marked with an asterisk (\*).

| Field             | Type               | Default    | Acuity UI Text |
| ----------------- | ------------------ | ---------- | -------------- |
| `project_token`\* | `text`             | `required` | Project Token  |
| `start_date`      | `date(yyyy-mm-dd)` | `nil`      | Start Date     |
| `end_date`        | `date(yyyy-mm-dd)` | `nil`      | Finish Date    |

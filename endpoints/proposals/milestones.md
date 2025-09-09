[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /proposals/milestones

**Description**: Retrieves a list of proposal milestones(not Scheduler) with performance indicators and custom colors.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/proposals/milestones`
- `url`: String, `https://<domain>/api/snapshot/proposals/milestones`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
  {
   "id": "integer",
   "name": "string",
   "description": "string",
   "project_id": "integer",
   "project_name": "string",
   "due_date": "date",
   "baseline_date": "date",
   "performance": "string",
   "performance_color": "string",
   "created_at": "date",
   "updated_at": "date"
   }
 ]
}
```


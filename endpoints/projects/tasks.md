[<- Back to List](https://github.com/AcuityPPM/APIs/blob/main/endpoints/list.md)

# API Endpoints

## GET /projects/tasks

**Description**: Retrieves a list of tasks.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/img/get_headers.webp)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/tasks`
- `url`: String, `https://<domain>/api/snapshot/projects/tasks`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
  {
   "id": "integer",
   "actual_finish_date": "date",
   "assigned_to": "string",
   "created_at": "date",
   "finish_date": "date",
   "notes": "text",
   "order_index": "integer",
   "performance": "green | yellow | red",
   "project_id": "integer",
   "project_name": "string",
   "start_date": "date",
   "status": "open | closed",
   "task_name": "string",
   "updated_at": "date"
   }
 ]
}
```


# API Endpoints

## GET /projects/resources

**Description**: Retrieves a list of project resources.

**Example Postman**:

![Alt text](image.png)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/resources`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
  {
   "id": "integer",
   "department": "null or string",
   "estimate": "integer",
   "end_date_planned": "date",
   "priority": "option",
   "project_name": "string",
   "project_resource_assignment_time_period_details": [
      {
        "id": "integer",
        "estimate": "integer",
        "month": "integer from 1 to 12",
        "year": "integer"
      },
   ],
   "resource_name": "string",
   "resource_role": "string",
   "risk_score": "integer",
   "start_date_planned": "date",
   "state": "option",
   "value_score": "integer",
   "Aug 2024": "integer",
   }
 ]
}

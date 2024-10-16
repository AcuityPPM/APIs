# API Endpoints

## GET /projects/lessons

**Description**: Retrieves a list of project lessons learned.

**Example Postman**:

![Alt text](https://github.com/AcuityPPM/APIs/blob/main/image.png)

- `domain`: String, ask `Acuity Support`
- `route`: String, `/projects/lessons`
- `Company-Api-Token`: UUID, ask `Acuity Support`

**Response**:

```json
{
 [
    {
        "id": "integer",
        "created_at": "date",
        "description": "string",
        "identified_by": "string",
        "impact": "string",
        "learned_lesson_options": "Lesson Options | null",
        "lesson_id": "integer",
        "lesson_learned": "string",
        "phase_name": "Phase Option | null",
        "project_id": "integer",
        "project_name": "string",
        "recommendation": "string",
        "updated_at": "date"
    }
 ]
}
```


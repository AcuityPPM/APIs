# API Endpoints

## GET /proposals

**Description**: Retrieves a list of users.

**Parameters**:

- `page`: Integer, optional, default=1
- `limit`: Integer, optional, default=10

**Response**:

```json
{
  "data": [
    {
      "id": 1,
      "name": "John Doe",
      ...
    },
    ...
  ],
  "meta": {
    "page": 1,
    "limit": 10,
    ...
  }
}

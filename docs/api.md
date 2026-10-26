# API reference

The API currently provides a single health-check endpoint.

## `GET /`

Returns a JSON message indicating that the API is running.

### Example

```powershell
curl.exe http://127.0.0.1:5000/
```

### Response

HTTP `200 OK`

```json
{
  "message": "Insurance Scheduler API is running"
}
```


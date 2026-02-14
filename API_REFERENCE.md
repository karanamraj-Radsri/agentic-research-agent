# API Reference

## Overview
This document provides comprehensive documentation for the API.

## Methods

### Method 1: `GET /example`
- **Parameters:** 
  - `param1` (string, required): Description of param1.
  - `param2` (int, optional): Description of param2.
- **Returns:** 
  - `200 OK`: Description of successful response structure.
  - `400 Bad Request`: Description of error when the request is invalid.

#### Example
```bash
curl -X GET "https://api.example.com/example?param1=value1&param2=10"
```

### Method 2: `POST /example`
- **Parameters:** 
  - `data` (object, required): JSON object with the data to be sent.
- **Returns:** 
  - `201 Created`: Description of created resource.
  - `500 Internal Server Error`: Description of server error.

#### Example
```bash
curl -X POST "https://api.example.com/example" -d '{"data":"value"}'
```

## Error Handling
- All error responses are returned in JSON format with the following structure:
  ```json
  {
    "error": "Error message",
    "code": "HTTP status code"
  }
  ```

## Rate Limits
- API usage is limited to 100 requests per minute.
- Exceeding the rate limit will result in a `429 Too Many Requests` response.

## Best Practices
- Always check for error responses and handle them appropriately.
- Use caching to reduce load on the API.
- Respect the rate limits to avoid disruptions in service.

## Conclusion
This API reference provides all necessary information to effectively utilize the API. For more details, refer to the individual method sections for specifics on parameters and responses.
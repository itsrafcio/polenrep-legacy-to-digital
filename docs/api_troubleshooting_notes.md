# API Troubleshooting Notes

## General approach

When an API request fails:

1. Define the expected result.
2. Check what actually happened.
3. Inspect the request:
   - HTTP method
   - URL
   - path parameters
   - query parameters
   - headers
   - authorization
   - request body
4. Inspect the response:
   - HTTP status code
   - response body
5. Form a hypothesis based on evidence.
6. Verify the hypothesis.
7. Fix and retest, or escalate if the problem is outside my control.

Do not diagnose an API problem based only on the HTTP status code.

## Error types reviewed

- 400 Bad Request — invalid request, data or format
- 401 Unauthorized — authentication problem
- 403 Forbidden — insufficient permissions
- 404 Not Found — endpoint or resource not found
- 409 Conflict — request conflicts with the current state of the system
- 429 Too Many Requests — rate limit exceeded
- 500 Internal Server Error — server-side error
- 502 Bad Gateway — problem between services or servers
- 503 Service Unavailable — service temporarily unavailable

## Practical lessons

- The response body often provides more useful information than the status code alone.
- A user-reported problem is not automatically a bug.
- Check whether the user's permissions match the business requirements.
- Do not make stronger claims than the evidence supports.
- If the problem is outside my control, provide Engineering with the request, response code and response body.
- Always retest after making a correction.
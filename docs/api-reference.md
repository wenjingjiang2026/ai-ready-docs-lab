# API reference (sample)

## POST /v1/chat

Request: `model` (string), `messages` (array).  
Response: `id`, `choices[].message.content`.  
Errors: `401` bad key, `404` unknown model, `429` rate limit.

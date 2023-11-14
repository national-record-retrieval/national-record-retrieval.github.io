<h1>get_order_status</h1>

| <p>Path</p> | <p class='remove_link'>https://nationalrr.com/api/index.php</p> |
| ----------- | --------------------------------------------------------------- |

<div class='api_container'>
<h2 class='left_title'>Payload Schema</h2>
<h2 class='right_title'>Example Payload</h2>
</div>

<div class='api_container'>

 <div class='api_schema'>
    <code>
{
  "type": "object",
  "properties": {
    "client_id": {
      "type": "string",
      "example": 1
    },
    "client_key": {
      "type": "string",
      "example": "key"
    },
    "request_type": {
      "type": "string",
      "example": "get_order_status"
    },
    "order_number": {
      "type": "string",
      "example": 722320
    },
    "user_email": {
      "type": "string",
      "example": "exampleuser@gmail.com"
    }
  },
  "required": [
    "client_id",
    "client_key",
    "request_type",
    "order_number",
    "user_email"
  ]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "client_id": "1",
  "client_key": "key",
  "request_type": "get_order_status",
  "order_number": "722320",
  "user_email": "exampleuser@gmail.com"
}
    </code>
  </div>

</div>

<div class='api_container'>
<h2 class='left_title'>Response Schema (200 OK)</h2>
<h2 class='right_title'>Example Response (200 OK)</h2>
</div>

<div class = 'api_container'>

  <div class='api_schema'>
    <code>
  "type": "string",
  "example": "Canceled",
  "description": "Status of order number in payload"
    </code>
  </div>

  <div class='api_response'>
    <code>
  "Canceled"
    </code>
  </div>

</div>

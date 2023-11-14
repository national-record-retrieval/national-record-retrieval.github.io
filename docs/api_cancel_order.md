<h1>cancel_order</h1>

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
    "request_type": {
      "type": "string",
      "example": "cancel_order"
    },
    "order_number": {
      "type": "integer",
      "example": 722318
    },
    "client_id": {
      "type": "integer",
      "example": 1
    },
    "client_key": {
      "type": "string",
      "example": "key"
    },
    "user_email": {
      "type": "string",
      "example": "exampleuser@gmail.com"
    }
  },
  "required": [
    "request_type",
    "order_number",
    "client_id",
    "client_key",
    "user_email"
  ]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request_type": "cancel_order",
  "order_number": 722318,
  "client_id": 1,
  "client_key": "key",
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
"example": "Order 722318 is canceled."
    </code>

  </div>

  <div class='api_response'>
    <code>
"Order 722318 is canceled."
    </code>
  </div>

</div>

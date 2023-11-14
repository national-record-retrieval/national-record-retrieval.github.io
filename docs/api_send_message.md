<h1>send_message</h1>

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
    "order_number": {
      "type": "integer",
      "example": 722320
    },
    "request_type": {
      "type": "string",
      "example": "send_message"
    },
    "message_receiver": {
      "type": "string",
      "example": "examplerecipient@gmail.com"
    },
    "action_method": {
      "type": "string",
      "example": "Email",
      "description": "method by which message is left"
    },
    "order_action": {
      "type": "string",
      "example": "Message"
    },
    "order_notes": {
      "type": "string",
      "example": "This is a test message recieved via api."
    }
  },
  "required": [
    "client_id",
    "client_key",
    "order_number",
    "request_type",
    "message_receiver",
    "action_method",
    "order_action"
  ]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "client_id": "1",
  "client_key": "key",
  "order_number": 722320,
  "request_type": "send_message",
  "message_receiver": "examplerecipient@gmail.com",
  "action_method": "Email",
  "order_action": "Message",
  "order_notes": "This is a test message recieved via api."
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
  "example": "Message sent."
    </code>
  </div>

  <div class='api_response'>
    <code>
  "Message sent."
    </code>
  </div>

</div>

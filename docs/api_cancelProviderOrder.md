<h1>cancelProviderOrder</h1>

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
    "request": {
      "type": "string",
      "example": "cancelProviderOrder"
    },
    "key": {
      "type": "string",
      "example": "key"
    },
    "user_email": {
      "type": "string",
      "example": "exampleuser@gmail.com"
    },
    "payload": {
      "type": "object",
      "properties": {
        "id": {
          "type": "integer",
          "example": 944581
        }
      },
      "required": ["id"]
    }
  },
  "required": ["request", "key", "user_email", "payload"]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request": "cancelProviderOrder",
  "key": "key",
  "user_email": "exampleuser@gmail.com",
  "payload": {
    "id": 944581
  }
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
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean",
      "example": true
    },
    "payload": {
      "type": "string",
      "example": null
    },
    "messages": {
      "type": "array",
      "items": {
        "type": "string",
        "example": "Provider order canceled."
      }
    },
    "warnings": {
      "type": "array",
      "items": {
        "type": "string"
      },
      "example": []
    },
    "errors": {
      "type": "array",
      "items": {
        "type": "string"
      },
      "example": []
    }
  }
}
    </code>
  </div>

  <div class='api_response'>
    <code>
{
  "success": true,
  "payload": null,
  "messages": [
    "Provider order canceled."
  ],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

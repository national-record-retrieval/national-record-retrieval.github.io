<h1>submitRetrievalOrder</h1>

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
      "example": "submitRetrievalOrder"
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
          "example": 735453,
          "description": "order id of unsubmitted order"
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
  "request": "submitRetrievalOrder",
  "key": "key",
  "user_email": "exampleuser@gmail.com",
  "payload": {
    "id": 735453
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
      "type": "object",
      "properties": {
        "orderId": {
          "type": "string",
          "example": 735453
        },
        "orderAction": {
          "type": "string",
          "example": "submit_order"
        },
        "messageType": {
          "type": "string",
          "example": null          
        },
        "valid": {
          "type": "string",
          "example": null
        },
        "invalidFields": {
          "type": "array",
          "items": {
            "type": "string"
          },
          "example": []
        }
      }
    },
    "messages": {
      "type": "array",
      "items": {
        "type": "string"
      },
      "example": []
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
  "payload": {
    "orderId": "735453",
    "orderAction": "submit_order",
    "messageType": "2023-10-19 14:21:07",
    "valid": null,
    "invalidFields": []
  },
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

<h1>get_order_state</h1>

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
      "example": "get_order_state"
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
  "request_type": "get_order_state",
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
{
    "type": "object",
    "properties": {
        "order": {
            "type": "object",
            "properties": {
                "id": {
                    "type": "string",
                    "example": "676415",
                    "description": "Order id"
                },
                "status": {
                    "type": "string",
                    "example": "Processing",
                    "description": "Order State"
                },
                "provider_order_rejected": {
                    "type": "integer",
                    "maximum": 1,
                    "minimum": 0,
                    "example": 0,
                    "description": "Indicates whether any provider order is rejected"
                },
                "provider_orders": {
                    "type": "array",
                    "items": {
                        "type": "object",
                        "properties": {
                            "id": {
                                "type": "string",
                                "example": "872640",
                                "description": "Provider Order id"
                            },
                            "rejected": {
                                "type": "string",
                                "maximum": "1",
                                "minimum": "0",
                                "example": "0",
                                "description": "Indicated whether the provider order is rejected"
                            },
                            "canceled": {
                                "type": "string",
                                "maximum": "1",
                                "minimum": "0",
                                "example": "0",
                                "description": "Indicated whether the provider order is canceled"
                            }
                        }
                    }
                }
            }
        }
    }
}
    </code>
  </div>

  <div class='api_response'>
    <code>
{
    "order": {
        "id": "676415",
        "status": "Processing",
        "provider_order_rejected": 0,
        "provider_orders": [
            {
                "id": "872640",
                "rejected": "0",
                "canceled": "0"
            },
            {
                "id": "872644",
                "rejected": "0",
                "canceled": "0"
            },
            {
                "id": "872645",
                "rejected": "0",
                "canceled": "0"
            },
            {
                "id": "873697",
                "rejected": "0",
                "canceled": "0"
            },
            {
                "id": "873707",
                "rejected": "0",
                "canceled": "0"
            }
        ]
    }
}
    </code>
  </div>

</div>

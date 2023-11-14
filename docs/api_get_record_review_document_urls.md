<h1>get_record_review_document_urls</h1>

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
      "example": "get_record_review_document_urls"
    },
    "client_id": {
      "type": "string",
      "example": 1
    },
    "client_key": {
      "type": "string",
      "example": "key"
    },
    "record_review_order_number": {
      "type": "string",
      "example": 12292
    },
    "user_email": {
      "type": "string",
      "example": "exampleuser@gmail.com"
    }
  },
  "required": [
    "request_type",
    "client_id",
    "client_key",
    "record_review_order_number",
    "user_email"
  ]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request_type": "get_record_review_document_urls",
  "client_id": "1",
  "client_key": "key",
  "record_review_order_number": "12292",
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
    "success": {
      "type": "boolean",
      "example": true
    },
    "payload": {
      "type": "array",
      "items": {
        "anyOf": [
          {
            "type": "object",
            "properties": {
              "document_id": {
                "type": "string",
                "example": 3392070
              },
              "presigned_url": {
                "type": "object",
                "properties": {
                  "url": {
                    "type": "string",
                    "example": "https://nrr-documents-dev-east.s3-accelerate.amazonaws.com/url"
                  },
                  "expiration_minutes": {
                    "type": "integer",
                    "example": 20
                  },
                  "generated_time": {
                    "type": "string",
                    "example": "10-18-2023 01:38:40"
                  }
                }
              }
            }
          }
        ]
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
  "payload": [
    {
      "document_id": "3392070",
      "presigned_url": {
        "url": "https://nrr-documents-dev-east.s3-accelerate.amazonaws.com/url",
        "expiration_minutes": 20,
        "generated_time": "10-18-2023 01:38:40"
      }
    }
  ]
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

<h1>get_document_urls</h1>

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
      "example": "get_document_urls"
    },
    "order_number": {
      "type": "string",
      "example": 735381
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
  "request_type": "get_document_urls",
  "order_number": "735381",
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
  "type": "array",
  "items": [
    {
      "type": "object",
      "properties": {
        "provider": {
          "type": "string",
          "example": "provider name"
        },
        "title": {
          "type": "string",
          "example": "returned_file_name.pdf"
        },
        "provider_order_id": {
          "type": "string",
          "example": 944509
        },
        "medical": {
          "type": "string",
          "example": 1,
          "description": "marked as medical document"
        },
        "lab": {
          "type": "string",
          "example": 0,
          "description": "marked as lab document"
        },
        "xrays": {
          "type": "string",
          "example": 0,
          "description": "marked as xrays document"
        },
        "bills": {
          "type": "string",
          "example": 0,
          "description": "marked as billing document"
        },
        "provider_order_complete": {
          "type": "string",
          "example": 1
        },
        "presigned_url": {
          "type": "object",
          "properties": {
            "url": {
              "type": "string",
              "example": "https://nrr-documents-dev-east.s3-accelerate.amazonaws.com/url"
            },
            "expiration_minutes": {
              "type": "string",
              "example": 20
            },
            "generated_time": {
              "type": "string",
              "example": "10-18-2023 09:51:50"
            }
          }
        }
      }
    }
  ]
}
    </code>

  </div>

  <div class='api_response'>
    <code>
[
  {
    "provider": "provider name",
    "title": "returned_file_name.pdf",
    "provider_order_id": "944509",
    "medical": "1",
    "lab": "0",
    "xrays": "0",
    "bills": "0",
    "provider_order_complete": "1",
    "presigned_url": {
      "url": "https://nrr-documents-dev-east.s3-accelerate.amazonaws.com/url",
      "expiration_minutes": "20",
      "generated_time": "10-18-2023 09:51:50"
    }
  },
  {
    "provider": "provider name",
    "title": "returned_file_name_2.pdf",
    "provider_order_id": "944509",
    "medical": "0",
    "lab": "0",
    "xrays": "0",
    "bills": "1",
    "provider_order_complete": "1",
    "presigned_url": {
      "url": "https://nrr-documents-dev-east.s3-accelerate.amazonaws.com/another-url",
      "expiration_minutes": "20",
      "generated_time": "10-18-2023 09:51:50"
    }
  }
]
    </code>

  </div>

</div>

<h1>newAuthorization_file_url</h1>

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
      "example": "newAuthorization"
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
        "order_id": {
          "type": "string",
          "example": 735452
        },
        "provider_order_id": {
          "type": "string",
          "example": 944581
        },
        "file_name": {
          "type": "string",
          "example": "Test.pdf"
        },
        "base_64": {
          "type": "string",
          "example": null
        },
        "file_url": {
          "type": "string",
          "example": "https://workflow-file-uploads.s3.us-west-2.amazonaws.com/url"
        }
      },
      "required": [
        "order_id",
        "provider_order_id",
        "file_name",
        "base_64",
        "file_url"
      ]
    }
  },
  "required": ["request", "key", "uer_email", "payload"]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request": "newAuthorization",
  "key": "key",
  "user_email": "exampleuser@gmail.com",
  "payload": {
    "order_id": "735452",
    "provider_order_id": "944581",
    "file_name": "Test.pdf",
    "base_64": null,
    "file_url": "https://workflow-file-uploads.s3.us-west-2.amazonaws.com/url"
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
        "id": {
          "type": "string",
          "example": 3428908,
          "description": "document id"
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
    "id": "3428908"
  },
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

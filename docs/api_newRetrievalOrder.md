<h1>newRetrievalOrder</h1>

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
      "example": "newRetrievalOrder"
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
        "patient_first": {
          "type": "string",
          "example": "Jane"
        },
        "patient_middle": {
          "type": "string",
          "example": "Elizabeth"
        },
        "patient_last": {
          "type": "string",
          "example": "Doe"
        },
        "patient_dob": {
          "type": "string",
          "format": "date",
          "example": "2022-01-01T00:00:00.000Z"
        },
        "patient_ssn": {
          "type": "string",
          "example": "123-13-1234"
        },
        "case_number": {
          "type": "string",
          "example": 20200723
        },
        "notes": {
          "type": "string",
          "example": "string"
        }
      },
      "required": ["patient_first", "patient_last", "patient_dob"]
    }
  },
  "required": ["request", "key", "user_email", "payload"]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request": "newRetrievalOrder",
  "key": "key",
  "user_email": "exampleuser@gmail.com",
  "payload": {
    "patient_first": "Jane",
    "patient_middle": "Elizabeth",
    "patient_last": "Doe",
    "patient_dob": "2022-01-01",
    "patient_ssn": "123-13-1234",
    "case_number": "20200723",
    "notes": "string"
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
          "example": 735419,
          "description": "order id"
        },
        "createdBy": {
          "type": "string",
          "example": 5674,
          "description": "user id"
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
    "id": "735419",
    "createdBy": "5674"
  },
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>

  </div>

</div>

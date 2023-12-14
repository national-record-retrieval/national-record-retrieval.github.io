<h1>provider_search</h1>

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
      "example": "provider_search"
    },
    "value": {
      "type": "string",
      "example": "Labcorp"
    },
    "client_id": {
      "type": "integer",
      "example": 1
    },
    "client_key": {
      "type": "string",
      "example": "key"
    }
  },
  "required": ["request_type", "value", "client_id", "client_key"]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request_type": "provider_search",
  "value": "Labcorp",
  "client_id": 1,
  "client_key": "key"
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
                "type": "object",
                "properties": {
                    "id": {
                        "type": "string",
                        "example": 6232,
                        "description": "provider id"
                    },
                    "provider_name": {
                        "type": "string",
                        "example": "LabCorp Dallas"
                    },
                    "location_id": {
                        "type": "string",
                        "example": 3601,
                        "description": "provider_location id"
                    },
                    "provider_street": {
                        "type": "string",
                        "example": "7777 Forest Lane, Suite C350",
                        "description": "provider street address"
                    },
                    "provider_city": {
                        "type": "string",
                        "example": "Dallas"
                    },
                    "provider_state": {
                        "type": "string",
                        "minLength": 2,
                        "maxLength": 2,
                        "example": "TX"
                    },
                    "provider_zip": {
                        "type": "string",
                        "minLength": 5,
                        "maxLength": 5,
                        "example": 75230
                    }
                }
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
    </code>

  </div>

  <div class='api_response'>
    <code>
{
  "success": true,
  "payload": [
    {
      "id": "6232",
      "provider_name": "LabCorp Dallas",
      "location_id": "3601",
      "provider_street": "7777 Forest Lane, Suite C350",
      "provider_city": "Dallas",
      "provider_state": "TX",
      "provider_zip": "75230"
    },
    {
      "id": "12103",
      "provider_name": "LabCorp Legal Department",
      "location_id": "9553",
      "provider_street": "1144 Pinehurst Dr",
      "provider_city": "Chapel Hill",
      "provider_state": "NC",
      "provider_zip": "27517"
    },
    {
      "id": "12110",
      "provider_name": "Labcorp - Sterling, VA",
      "location_id": "9559",
      "provider_street": "47100 Community Plaza",
      "provider_city": "Sterling",
      "provider_state": "VA",
      "provider_zip": "20164"
    },
    {
      "id": "12591",
      "provider_name": "Labcorp- Midlothian",
      "location_id": "10054",
      "provider_street": "5610 West LaSalle Street",
      "provider_city": "Tampa",
      "provider_state": "FL",
      "provider_zip": "33607"
    }
  ],
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>

  </div>

</div>

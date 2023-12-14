<h1>get_torts</h1>

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
            "example": "get_torts"
        },
        "client_id": {
            "type": "integer",
            "example": 1
        },
        "client_key": {
            "type": "string",
            "example": "key"
        }
    }
},
"required": ["request_type", "client_id", "client_key"]
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request_type": "get_torts",
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
            "type": "boolean"
        },
        "payload": {
            "type": "array",
            "items": {
                "type": "object",
                "properties": {
                    "id": {
                        "type": "string",
                        "example": "26"
                    },
                    "name": {
                        "type": "string",
                        "example": "Medical Malpractice"
                    },
                    "position": {
                        "type": "string",
                        "example": "1"
                    }
                }
            }
        }
    },
    "messages": {
        "type": "array",
        "example": []
    },
    "warnings": {
        "type": "array",
        "example": []
    },
    "errors": {
        "type": "array",
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
      "id": "26",
      "name": "Medical Malpractice",
      "position": "1"
    },
    {
      "id": "1",
      "name": "Personal Injury",
      "position": "2"
    },
    {
      "id": "27",
      "name": "Product Liability",
      "position": "3"
    },
    {
      "id": "3",
      "name": "3M Earplugs",
      "position": "4"
    },
    {
      "id": "2",
      "name": "Camp Lejune Ed",
      "position": "5"
    },
    {
      "id": "4",
      "name": "Elmiron",
      "position": "6"
    },
    {
      "id": "30",
      "name": "Exactech",
      "position": "7"
    },
    {
      "id": "8",
      "name": "Firefighter Foam (AFFF)",
      "position": "8"
    },
    {
      "id": "12",
      "name": "Gardasil",
      "position": "9"
    },
    {
      "id": "19",
      "name": "Hair Straightener",
      "position": "10"
    },
    {
      "id": "7",
      "name": "Heavy Metal Baby Food",
      "position": "11"
    },
    {
      "id": "9",
      "name": "Hernia Mesh",
      "position": "12"
    },
    {
      "id": "32",
      "name": "Injectafer",
      "position": "13"
    },
    {
      "id": "25",
      "name": "IVC Filter",
      "position": "14"
    },
    {
      "id": "6",
      "name": "NEC Baby Formula",
      "position": "15"
    },
    {
      "id": "18",
      "name": "Opioids",
      "position": "16"
    },
    {
      "id": "14",
      "name": "Paraguard IUD",
      "position": "17"
    },
    {
      "id": "13",
      "name": "Paraquat",
      "position": "18"
    },
    {
      "id": "28",
      "name": "PFAS",
      "position": "19"
    },
    {
      "id": "11",
      "name": "Phillips CPAP",
      "position": "20"
    },
    {
      "id": "10",
      "name": "Roundup",
      "position": "21"
    },
    {
      "id": "16",
      "name": "Talcum Powder",
      "position": "22"
    },
    {
      "id": "5",
      "name": "Tylenol",
      "position": "23"
    },
    {
      "id": "15",
      "name": "Zantac",
      "position": "24"
    },
    {
      "id": "31",
      "name": "Tepezza",
      "position": "25"
    }
  ],
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

<h1>submit_order</h1>

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
      "example": "submit_order"
    },
    "patient_first_name": {
      "type": "string",
      "example": "Jane"
    },
    "patient_middle_name": {
      "type": "string",
      "example": "Elizabeth"
    },
    "patient_last_name": {
      "type": "string",
      "example": "Doe"
    },
    "patient_dob": {
      "type": "string",
      "format": "YYYY-MM-DD",
      "example": "2001-01-01"
    },
    "patient_ssn": {
      "type": "string",
      "format": "SSN",
      "example": "123-13-1234"
    },
    "case_number": {
      "type": "string",
      "example": 20200273
    },
    "patient_notes": {
      "type": "string",
      "example": "This is a patient note"
    },
    "rush_order": {
      "type": "integer",
      "minimum": 0,
      "maximum": 1,
      "example": 0
    },
    "providers": {
      "type": "array",
      "items": {
        "type": "array",
        "items": {
          "anyOf": [
            {
              "type": "string",
              "example": "Provider Name"
            },
            {
              "type": "string",
              "example": "Provider Address"
            },
            {
              "type": "string",
              "format": "YYYY-MM-DD",
              "description": "Service start date",
              "example": "2001-01-01"
            },
            {
              "type": "string",
              "format": "YYYY-MM-DD",
              "description": "Service end date",
              "example": "2099-01-01"
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Record Type - Medical",
              "example": 1
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Record Type - Bills",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Record Type - X-Rays",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Record Type - Lab",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Certify Records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "All Dates",
              "example": 0
            },
            {
              "type": "string",
              "example": "This is a provider note",
              "description": "provider note"
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - abstract_medical_records"
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - admissions_face_sheet",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - ambulance_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - attending_physicians_statement",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - autopsy_reports",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - anesthesia_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - chart_stickers",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - consultation_reports",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - discharge_summary",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - doctors_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - er_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - fetal_monitoring_strips",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - gastrointestinal_lab_reports",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - history_physical_reports",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - implant_explant_logs",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 0,
              "description": "Med Subtype - intra_operative_nursing_notes"
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - laboratory_reports",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - nurses_notes",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - nurses_medication_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - office_notes",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - operative_reports",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - pathology_reports",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - pharmacy_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - photographs",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - physical_therapy_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - preop_standing_orders",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - product_id_implant_label",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - psychiatric_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype radiology_diagnostic_reports",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Med Subtype - recovery_room_records",
              "example": 0
            },
            {
              "type": "integer",
              "minimum": 0,
              "maximum": 1,
              "description": "Rush Records",
              "example": 0
            }
          ]
        }
      }
    },
    "documents": {
      "type": "array",
      "items": {
        "type": "array",
        "items": {
          "anyOf": [
            {
              "type": "string",
              "description": "File Name",
              "example": "FileName.pdf"
            },
            {
              "type": "string",
              "example": 29800,
              "description": "File Size"
            },
            {
              "type": "string",
              "example": 2,
              "description": `File affiliation 1:"Uncategorized", 2:"Medical" 3:"Lab", 4:"Radiology", 5:"Billing"`
            },
            {
              "type": "string",
              "example": "data:@file/pdf;base64 ...",
              "description": "Base 64 corresponding to the file"
            }
          ]
        }
      }
    },
    "client_id": {
      "type": "integer",
      "example": 1
    },
    "client_key": {
      "type": "string",
      "example": "key"
    },
    "user_email": {
      "type": "string",
      "example": "exampleuser@gmail.com"
    }
  },
  "required": [
    "request_type",
    "patient_first_name",
    "patient_last_name",
    "patient_dob",
    "providers"
  ]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request_type": "submit_order",
  "patient_first_name": "Jane",
  "patient_middle_name": "Elizabeth",
  "patient_last_name": "Doe",
  "patient_dob": "2001-01-01",
  "patient_ssn": "123-13-1234",
  "case_number": "20200273",
  "patient_notes": "This is a patient note",
  "rush_order": 0,
  "providers": [
    [
      "Provider Name",
      "Provider Address",
      "2001-01-01",
      "2099-01-01",
      1,
      0,
      0,
      0,
      0,
      0,
      "This is a provider note",
      1,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0,
      0
    ]
  ],
  "documents": [
    [
      "FileName.pdf",
      "29800",
      "2",
      "data:@file/pdf;base64"
    ]
  ],
  "client_id": 1,
  "client_key": "key",
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
  "type": "string",
  "example": 735407,
  "description": "order number of created order"
    </code>
  </div>

  <div class='api_response'>
    <code>
  "735407"
    </code>
  </div>

</div>

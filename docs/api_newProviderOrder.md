<h1>newProviderOrder</h1>

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
      "example": "newProviderOrder"
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
          "type": "integer",
          "example": 732949
        },
        "all_dates": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0
        },
        "service_start": {
          "type": "string",
          "format": "date",
          "example": "2001-01-01T00:00:00.000Z"
        },
        "service_end": {
          "type": "string",
          "format": "date",
          "example": "2023-01-01T00:00:00.000Z"
        },
        "provider_name": {
          "type": "string",
          "example": "My Provider Name"
        },
        "provider_address": {
          "type": "string",
          "example": "123 My Place, Peoria, IL 61605"
        },
        "certified_records": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 1
        },
        "rush_order": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 1
        },
        "notes": {
          "type": "string",
          "example": "This is a provider note"
        },
        "record_types": {
          "type": "object",
          "properties": {
            "medical": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 1
            },
            "lab": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 1
            },
            "xrays": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 1
            },
            "bills": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": "1'"
            }
          }
        },
        "medical_subtypes": {
          "type": "object",
          "properties": {
            "abstract_medical_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "admissions_face_sheet": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "ambulance_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "attending_physicians_statement": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "autopsy_reports": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "anethesia_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "chart_stickers": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "consultation_reports": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "discharge_summary": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "doctors_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "er_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "fetal_monitoring_strips": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "gastrointestinal_lab_reports": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "history_physical_reports": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "implant_explant_logs": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "intra_operative_nursing_notes": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "laboratory_reports": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "nurses_notes": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "nurses_medication_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "office_notes": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "operative_reports": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "pathology_reports": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "pharmacy_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "photographs": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "physical_therapy_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "preop_standing_orders": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "product_id_implant_label": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "psychiatric_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "radiology_diagnostic_reports": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            },
            "recovery_room_records": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0
            }
          }
        }
      },
      "required": [
        "order_id",
        "all_dates",
        "provider_name",
        "provider_address",
        "record_types"
      ]
    }
  },
  "required": ["request", "key", "user_email", "payload"]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request": "newProviderOrder",
  "key": "key",
  "user_email": "exampleuser@gmail.com",
  "payload": {
    "order_id": 732949,
    "all_dates": 0,
    "service_start": "2001-01-01",
    "service_end": "2023-01-01",
    "provider_name": "My Provider Name",
    "provider_address": "123 My Place, Peoria, IL 61605",
    "certified_records": 1,
    "rush_order": 1,
    "notes": "This is a provider note",
    "record_types": {
      "medical": 1,
      "lab": 1,
      "xrays": 1,
      "bills": "1'"
    },
    "medical_subtypes": {
      "abstract_medical_records": 0,
      "admissions_face_sheet": 0,
      "ambulance_records": 0,
      "attending_physicians_statement": 0,
      "autopsy_reports": 0,
      "anethesia_records": 0,
      "chart_stickers": 0,
      "consultation_reports": 0,
      "discharge_summary": 0,
      "doctors_records": 0,
      "er_records": 0,
      "fetal_monitoring_strips": 0,
      "gastrointestinal_lab_reports": 0,
      "history_physical_reports": 0,
      "implant_explant_logs": 0,
      "intra_operative_nursing_notes": 0,
      "laboratory_reports": 0,
      "nurses_notes": 0,
      "nurses_medication_records": 0,
      "office_notes": 0,
      "operative_reports": 0,
      "pathology_reports": 0,
      "pharmacy_records": 0,
      "photographs": 0,
      "physical_therapy_records": 0,
      "preop_standing_orders": 0,
      "product_id_implant_label": 0,
      "psychiatric_records": 0,
      "radiology_diagnostic_reports": 0,
      "recovery_room_records": 0
    }
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
          "example": 944583,
          "description": "provider order id"
        },
        "addedBy": {
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
    "id": "944583",
    "addedBy": "5674"
  },
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

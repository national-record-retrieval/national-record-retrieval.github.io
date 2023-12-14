<h1>submit_record_review_order</h1>

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
      "example": "submit_record_review_order"
    },
    "client_id": {
      "type": "string",
      "example": 1
    },
    "client_key": {
      "type": "string",
      "example": "key"
    },
    "user_email": {
      "type": "string",
      "example": "exampleuser@gmail.com"
    },
    "patientFirst": {
      "type": "string",
      "example": "Test First Name"
    },
    "PatientMiddle": {
      "type": "string",
      "example": "Test Middle Name"
    },
    "PatientLast": {
      "type": "string",
      "example": "Test Last Name"
    },
    "caseNumber": {
      "type": "string",
      "example": "test-001"
    },
    "services": {
      "type": "object",
      "properties": {
        "standardSummary": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for standard summary"
        },
        "recordHighlights": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for record highlights"
        },
        "chronology": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for chronology"
        },
        "caseEvaluation": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 1,
          "description": "marked for case evaluation"
        },
        "plaintiffFactSheet": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for plaintiff fact sheet"
        },
        "demandLetters": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for demand letters"
        },
        "medicalExpenses": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for medical expenses"
        },
        "medicalSynopsis": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for medical synopsis"
        },
        "painSufferingChart": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for pain and suffering chart"
        },
        "narrativeSummary": {
          "type": "integer",
          "maximum": 1,
          "minimum": 0,
          "example": 0,
          "description": "marked for narrative summary"
        }
      }
    },
    "instructions": {
      "type": "string",
      "example": "review instructions"
    },
    "tortId": {
      "type": "string",
      "example": 10
    },
    "records": {
      "type": "array",
      "items": [
        {
          "type": "object",
          "properties": {
            "fileName": {
              "type": "string",
              "example": "testfile.pdf"
            },
            "fileSize": {
              "type": "integer",
              "example": 1321
            },
            "base64": {
              "type": "string",
              "example": "@file/pdf;base64,base64"
            }
          },
          "required": ["fileName", "fileSize", "base64"]
        },
        {
          "type": "object",
          "properties": {
            "id": {
              "type": "integer",
              "example": 2293708,
              "description": "document id"
            }
          },
          "required": ["id"]
        }
      ]
    },
    "api": {
      "type": "integer",
      "example": 1
    }
  },
  "required": [
    "request_type",
    "client_id",
    "client_key",
    "user_email",
    "patient_first",
    "patient_last",
    "services",
    "tortId"
  ]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request_type": "submit_record_review_order",
  "client_id": "1",
  "client_key": "key",
  "user_email": "exampleuser@gmail.com",
  "patientFirst": "Test First Name",
  "PatientMiddle": "Test Middle Name",
  "PatientLast": "Test Last Name",
  "caseNumber": "test-001",
  "services": {
    "standardSummary": 0,
    "recordHighlights": 0,
    "chronology": 0,
    "caseEvaluation": 1,
    "plaintiffFactSheet": 0,
    "demandLetters": 0,
    "medicalExpenses": 0,
    "medicalSynopsis": 0,
    "painSufferingChart": 0,
    "narrativeSummary": 0
  },
  "instructions": "review instructions",
  "tortId": "10",
  "records": [
    {
      "fileName": "testfile.pdf",
      "fileSize": 1321,
      "base64": "@file/pdf;base64,base64"
    },
    {
      "id": 2293708
    }
  ],
  "api": 1
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
        "patientFirst": {
          "type": "string",
          "example": "Test First Name"
        },
        "PatientMiddle": {
          "type": "string",
          "example": "Test Middle Name"
        },
        "PatientLast": {
          "type": "string",
          "example": "Test Last Name"
        },
        "caseNumber": {
          "type": "string",
          "example": "test-001"
        },
        "services": {
          "type": "object",
          "properties": {
            "patientFirst": {
              "type": "string",
              "example": "Test First Name"
            },
            "patientMiddle": {
              "type": "string",
              "example": "Test Middle Name"
            },
            "patientLast": {
              "type": "string",
              "example": "Test Last Name"
            },
            "caseNumber": {
              "type": "string",
              "example": "test-001"
            },
            "standardSummary": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for standard summary"
            },
            "recordHighlights": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for record highlights"
            },
            "chronology": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for chronology"
            },
            "caseEvaluation": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 1,
              "description": "marked for case evaluation"
            },
            "plaintiffFactSheet": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for plaintiff fact sheet"
            },
            "demandLetters": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for demand letters"
            },
            "medicalExpenses": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for medical expenses"
            },
            "medicalSynopsis": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for medical synopsis"
            },
            "painSufferingChart": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for pain and suffering chart"
            },
            "narrativeSummary": {
              "type": "integer",
              "maximum": 1,
              "minimum": 0,
              "example": 0,
              "description": "marked for narrative summary"
            },
            "instructions": {
              "type": "string",
              "example": "review instructions"
            },
            "tortId": {
              "type": "string",
              "example": 10
            },
            "assignedTo": {
              "type": "string",
              "example": null
            },
            "tort": {
              "type": "string",
              "example": null
            },
            "records": {
              "type": "string",
              "example": null
            },
            "review": {
              "type": "object",
              "properties": {
                "orderId": {
                  "type": "string",
                  "example": 12346
                },
                "status": {
                  "type": "string",
                  "example": "pending"
                },
                "notes": {
                  "type": "string",
                  "example": null
                },
                "fees": {
                  "type": "array",
                  "items": {
                    "type": "string"
                  },
                  "example": []
                },
                "records": {
                  "type": "array",
                  "items": {
                    "type": "string"
                  },
                  "example": []
                },
                "addedBy": {
                  "type": "string",
                  "example": 5674,
                  "description": "user id"
                },
                "addedDate": {
                  "type": "string",
                  "example": "2023-10-18T16:53:42.000Z"
                },
                "modifiedBy": {
                  "type": "string",
                  "example": 6574,
                  "description": "user id"
                },
                "modifiedDate": {
                  "type": "string",
                  "example": "2023-10-18T16:53:42.000Z"
                },
                "dataPoints": {
                  "type": "array",
                  "items": {
                    "type": "string"
                  },
                  "example": []
                },
                "tort": {
                  "type": "array",
                  "items": {
                    "type": "string"
                  },
                  "example": []
                },
                "id": {
                  "type": "string",
                  "example": 12346,
                  "description": "record review id"
                },
                "service": {
                  "type": "string",
                  "example": null
                },
                "valid": {
                  "type": "string",
                  "example": null
                },
                "invalidFields:": {
                  "type": "array",
                  "items": {
                    "type": "string"
                  },
                  "example": []
                }
              }
            },
            "recordDataPoints": {
              "type": "array",
              "items": {
                "type": "string"
              },
              "example": []
            },
            "id": {
              "type": "string",
              "example": 12346
            },
            "service": {
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
    "patientFirst": "Test First Name",
    "PatientMiddle": "Test Middle Name",
    "PatientLast": "Test Last Name",
    "caseNumber": "test-001",
    "services": {
      "patientFirst": "Test First Name",
      "patientMiddle": "Test Middle Name",
      "patientLast": "Test Last Name",
      "caseNumber": "test-001",
      "standardSummary": 0,
      "recordHighlights": 0,
      "chronology": 0,
      "caseEvaluation": 1,
      "plaintiffFactSheet": 0,
      "demandLetters": 0,
      "medicalExpenses": 0,
      "medicalSynopsis": 0,
      "painSufferingChart": 0,
      "narrativeSummary": 0,
      "instructions": "review instructions",
      "tortId": "10",
      "assignedTo": null,
      "tort": null,
      "records": null,
      "review": {
        "orderId": "12346",
        "status": "pending",
        "notes": null,
        "fees": [],
        "records": [],
        "addedBy": "5674",
        "addedDate": "2023-10-18 16:53:42",
        "modifiedBy": "6574",
        "modifiedDate": "2023-10-18 16:53:42",
        "dataPoints": [],
        "tort": [],
        "id": "12346",
        "service": null,
        "valid": null,
        "invalidFields:": []
      },
      "recordDataPoints": [],
      "id": "12346",
      "service": null,
      "valid": null,
      "invalidFields": []
    }
  },
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

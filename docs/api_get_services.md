<h1>get_services</h1>

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
      "example": "get_services"
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
  "required": ["request_type", "client_id", "client_key"]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request_type": "get_services",
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
        "anyOf": [
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Medical Record Review"
              },
              "description": {
                "type": "string",
                "example": "Features chronological summary of records highlighting chief complaint, history of present illness, past medical/surgical history, family history, assessment/plan, exam, etc.  Record is hyperlinked."
              },
              "documentPath": {
                "type": "string",
                "example": "./file_downloads/NRRSample1.pdf"
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "standard_summary"
              },
              "id": {
                "type": "string",
                "example": 1
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Medical Record Review w/Bookmarks"
              },
              "description": {
                "type": "string",
                "example": "Features chronological summary of records highlighting chief complaint, history of present illness, past medical/surgical history, family history, assessment/plan, exam, etc. Record is hyperlinked AND bookmarked for easiest navigation."
              },
              "documentPath": {
                "type": "string",
                "example": "./file_downloads/NRRSample3.pdf"
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "chronology"
              },
              "id": {
                "type": "string",
                "example": 2
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Record Highlights"
              },
              "description": {
                "type": "string",
                "example": "Key components of record are highlighted, hyperlinked, and bookmarked. Traditional summarization is not provided. This is a “lite” option geared towards cost-effective mass tort record review. Custom components and formatting can be formulated and set with NRR per tort type for easy repeat ordering."
              },
              "documentPath": {
                "type": "string",
                "example": "./file_downloads/HighlightsSample.pdf"
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "record_highlights"
              },
              "id": {
                "type": "string",
                "example": 3
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Medical Expense / Billing Summary"
              },
              "description": {
                "type": "string",
                "example": "Medical bills are sorted in chronological order and expenses are itemized in a spreadsheet including dates of treatment, types of treatment rendered and expenses incurred."
              },
              "documentPath": {
                "type": "string",
                "example": ""
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "medical_expenses"
              },
              "id": {
                "type": "string",
                "example": 4
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Pain and Suffering Chart"
              },
              "description": {
                "type": "string",
                "example": "Shows pain and suffering objectively through colorful charts that depict the spike in pain med prescriptions post-accident. Ideal as demonstrative evidence for Demand Letters, Mediation and Trial."
              },
              "documentPath": {
                "type": "string",
                "example": ""
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "pain_suffering_chart"
              },
              "id": {
                "type": "string",
                "example": 5
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Mass-Tort Case Evaluation"
              },
              "description": {
                "type": "string",
                "example": "Record review to determine mass tort case viability. NRR will work with you to define your firm’s specific qualification parameters for each tort."
              },
              "documentPath": {
                "type": "string",
                "example": ""
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "case_evaluation"
              },
              "id": {
                "type": "string",
                "example": 6
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Plaintiff Fact Sheet"
              },
              "description": {
                "type": "string",
                "example": "Completion of the MDL’s standardized form with your client’s information."
              },
              "documentPath": {
                "type": "string",
                "example": ""
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "plaintiff_fact_sheet"
              },
              "id": {
                "type": "string",
                "example": 7
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Demand Letters (ICD Codes)"
              },
              "description": {
                "type": "string",
                "example": "Presents facts about the accident to persuade the insurance adjuster to provide fair compensation. Includes a factual summary and details injuries including pain & suffering, treatments, medical bills, and lost income along with liability."
              },
              "documentPath": {
                "type": "string",
                "example": ""
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "demand_letters"
              },
              "id": {
                "type": "string",
                "example": 8
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Medical Synopsis"
              },
              "description": {
                "type": "string",
                "example": "Provides a chronological informative overview of the claimant’s medical history. Use the Medical Synopsis we provide to learn what happened to the patient and determine the merit of the case. Includes every relevant visit, a short narrative, highlights any major events, and can be customized to suit your needs."
              },
              "documentPath": {
                "type": "string",
                "example": ""
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "medical_synopsis"
              },
              "id": {
                "type": "string",
                "example": 9
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
          },
          {
            "type": "object",
            "properties": {
              "name": {
                "type": "string",
                "example": "Narrative Summary"
              },
              "description": {
                "type": "string",
                "example": "A brief flow of events in the patient’s health history that help to understand the overall case in a short format."
              },
              "documentPath": {
                "type": "string",
                "example": "./file_downloads/NarrativeSummarySample.pdf"
              },
              "recordReviewColumn": {
                "type": "string",
                "example": "narrative_summary"
              },
              "id": {
                "type": "string",
                "example": 10
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
      "name": "Medical Record Review",
      "description": "Features chronological summary of records highlighting chief complaint, history of present illness, past medical/surgical history, family history, assessment/plan, exam, etc.  Record is hyperlinked.",
      "documentPath": "./file_downloads/NRRSample1.pdf",
      "recordReviewColumn": "standard_summary",
      "id": "1",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Medical Record Review w/Bookmarks",
      "description": "Features chronological summary of records highlighting chief complaint, history of present illness, past medical/surgical history, family history, assessment/plan, exam, etc. Record is hyperlinked AND bookmarked for easiest navigation.",
      "documentPath": "./file_downloads/NRRSample3.pdf",
      "recordReviewColumn": "chronology",
      "id": "2",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Record Highlights",
      "description": "Key components of record are highlighted, hyperlinked, and bookmarked. Traditional summarization is not provided. This is a “lite” option geared towards cost-effective mass tort record review. Custom components and formatting can be formulated and set with NRR per tort type for easy repeat ordering.",
      "documentPath": "./file_downloads/HighlightsSample.pdf",
      "recordReviewColumn": "record_highlights",
      "id": "3",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Medical Expense / Billing Summary",
      "description": "Medical bills are sorted in chronological order and expenses are itemized in a spreadsheet including dates of treatment, types of treatment rendered and expenses incurred.",
      "documentPath": "",
      "recordReviewColumn": "medical_expenses",
      "id": "4",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Pain and Suffering Chart",
      "description": "Shows pain and suffering objectively through colorful charts that depict the spike in pain med prescriptions post-accident. Ideal as demonstrative evidence for Demand Letters, Mediation and Trial.",
      "documentPath": "",
      "recordReviewColumn": "pain_suffering_chart",
      "id": "5",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Mass-Tort Case Evaluation",
      "description": "Record review to determine mass tort case viability. NRR will work with you to define your firm’s specific qualification parameters for each tort.",
      "documentPath": "",
      "recordReviewColumn": "case_evaluation",
      "id": "6",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Plaintiff Fact Sheet",
      "description": "Completion of the MDL’s standardized form with your client’s information.",
      "documentPath": "",
      "recordReviewColumn": "plaintiff_fact_sheet",
      "id": "7",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Demand Letters (ICD Codes)",
      "description": "Presents facts about the accident to persuade the insurance adjuster to provide fair compensation. Includes a factual summary and details injuries including pain & suffering, treatments, medical bills, and lost income along with liability.",
      "documentPath": "",
      "recordReviewColumn": "demand_letters",
      "id": "8",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Medical Synopsis",
      "description": "Provides a chronological informative overview of the claimant’s medical history. Use the Medical Synopsis we provide to learn what happened to the patient and determine the merit of the case. Includes every relevant visit, a short narrative, highlights any major events, and can be customized to suit your needs.",
      "documentPath": "",
      "recordReviewColumn": "medical_synopsis",
      "id": "9",
      "service": null,
      "valid": null,
      "invalidFields": []
    },
    {
      "name": "Narrative Summary",
      "description": "A brief flow of events in the patient’s health history that help to understand the overall case in a short format.",
      "documentPath": "./file_downloads/NarrativeSummarySample.pdf",
      "recordReviewColumn": "narrative_summary",
      "id": "10",
      "service": null,
      "valid": null,
      "invalidFields": []
    }
  ],
  "messages": [],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

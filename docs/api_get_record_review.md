<h1>get_record_review</h1>

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
      "example": "get_record_review"
    },
    "client_id": {
      "type": "string",
      "example": 1
    },
    "client_key": {
      "type": "string",
      "example": "key"
    },
    "record_review_id": {
      "type": "integer",
      "example": 12364
    },
    "user_email": {
      "type": "integer",
      "example": "exampleuser@gmail.com"
    }
  },
  "required": [
    "request_type",
    "client_id",
    "client_key",
    "record_review_id",
    "user_email"
  ]
}
    </code>

  </div>

  <div class='api_payload'>
    <code>
{
  "request_type": "get_record_review",
  "client_id": "1",
  "client_key": "key",
  "record_review_id": 12364,
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
      "type": "object",
      "properties": {
        "orderId": {
          "type": "string",
          "example": 12364
        },
        "status": {
          "type": "string",
          "example": "complete"
        },
        "addedBy": {
          "type": "string",
          "example": 3885,
          "description": "user id"
        },
        "addedDate": {
          "type": "string",
          "example": "2023-10-12T10:21:43.000Z"
        },
        "modifiedBy": {
          "type": "string",
          "example": 5998,
          "description": "user id"
        },
        "modifiedDate": {
          "type": "string",
          "example": "20023-10-18 13:11:59"
        },
        "dataPoints": {
          "type": "object",
          "properties": {
            "0": {
              "type": "object",
              "properties": {
                "label": {
                  "type": "string",
                  "example": "Side Effects"
                },
                "type": {
                  "type": "string",
                  "example": "textarea"
                },
                "field_name": {
                  "type": "string",
                  "example": "side_effects"
                },
                "value": {
                  "type": "string",
                  "example": "Side Effect Data"
                }
              }
            },
            "Products": {
              "type": "array",
              "items": {
                "anyOf": [
                  {
                    "type": "array",
                    "items": {
                      "anyOf": [
                        {
                          "type": "object",
                          "properties": {
                            "label": {
                              "type": "string",
                              "example": "Product Used"
                            },
                            "type": {
                              "type": "string",
                              "example": "text"
                            },
                            "field_name": {
                              "type": "string",
                              "example": "product_used"
                            },
                            "value": {
                              "type": "string",
                              "example": "Product Used Data"
                            }
                          }
                        },
                        {
                          "type": "object",
                          "properties": {
                            "label": {
                              "type": "string",
                              "example": "Product UPC"
                            },
                            "type": {
                              "type": "string",
                              "example": "text"
                            },
                            "field_name": {
                              "type": "string",
                              "example": "product_upc"
                            },
                            "value": {
                              "type": "string",
                              "example": "Product UPC data"
                            }
                          }
                        },
                        {
                          "type": "object",
                          "properties": {
                            "label": {
                              "type": "string",
                              "example": "Product Dosage"
                            },
                            "type": {
                              "type": "string",
                              "example": "text"
                            },
                            "field_name": {
                              "type": "string",
                              "example": "product_dosage"
                            },
                            "value": {
                              "type": "string",
                              "example": "product dosage data"
                            }
                          }
                        },
                        {
                          "type": "object",
                          "properties": {
                            "label": {
                              "type": "string",
                              "example": "Began Usage"
                            },
                            "type": {
                              "type": "string",
                              "example": "date"
                            },
                            "field_name": {
                              "type": "string",
                              "example": "began_usage"
                            },
                            "value": {
                              "type": "string",
                              "format": "date",
                              "example": "2022-12-31T00:00:00.000Z"
                            }
                          }
                        },
                        {
                          "type": "object",
                          "properties": {
                            "label": {
                              "type": "string",
                              "example": "Ended Usage"
                            },
                            "type": {
                              "type": "string",
                              "example": "date"
                            },
                            "field_name": {
                              "type": "string",
                              "example": "ended_usage"
                            },
                            "value": {
                              "type": "string",
                              "format": "date",
                              "example": "2023-12-31T00:00:00.000Z"
                            }
                          }
                        }
                      ]
                    }
                  }
                ]
              }
            },
            "Outcomes": {
              "type": "array",
              "items": {
                "type": "array",
                "items": {
                  "anyOf": [
                    {
                      "type": "object",
                      "properties": {
                        "label": {
                          "type": "string",
                          "example": "Outcome"
                        },
                        "type": {
                          "type": "string",
                          "example": "text"
                        },
                        "field_name": {
                          "type": "string",
                          "example": "outcome"
                        },
                        "value": {
                          "type": "string",
                          "example": "Outcome Data"
                        }
                      }
                    },
                    {
                      "type": "object",
                      "properties": {
                        "label": {
                          "type": "string",
                          "example": "ICD code"
                        },
                        "type": {
                          "type": "string",
                          "example": "text"
                        },
                        "field_name": {
                          "type": "string",
                          "example": "icd_code"
                        },
                        "value": {
                          "type": "string",
                          "example": "ICD code Data"
                        }
                      }
                    },
                    {
                      "type": "object",
                      "properties": {
                        "label": {
                          "type": "string",
                          "example": "Symptoms"
                        },
                        "type": {
                          "type": "string",
                          "example": "textarea"
                        },
                        "field_name": {
                          "type": "string",
                          "example": "symptoms"
                        },
                        "value": {
                          "type": "string",
                          "example": "Symptoms data"
                        }
                      }
                    }
                  ]
                }
              }
            }
          }
        },
        "id": {
          "type": "string",
          "example": 12364,
          "description": "record review id"
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
    "message": {
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
    "orderId": "12364",
    "status": "complete",
    "addedBy": "3885",
    "addedDate": "2023-10-12 10:21:43",
    "modifiedBy": "5998",
    "modifiedDate": "20023-10-18 13:11:59",
    "dataPoints": {
      "0": {
        "label": "Side Effects",
        "type": "textarea",
        "field_name": "side_effects",
        "value": "Side Effect Data"
      },
      "Products": [
        [
          {
            "label": "Product Used",
            "type": "text",
            "field_name": "product_used",
            "value": "Product Used Data"
          },
          {
            "label": "Product UPC",
            "type": "text",
            "field_name": "product_upc",
            "value": "Product UPC data"
          },
          {
            "label": "Product Dosage",
            "type": "text",
            "field_name": "product_dosage",
            "value": "product dosage data"
          },
          {
            "label": "Began Usage",
            "type": "date",
            "field_name": "began_usage",
            "value": "2022-12-31"
          },
          {
            "label": "Ended Usage",
            "type": "date",
            "field_name": "ended_usage",
            "value": "2023-12-31"
          }
        ]
      ],
      "Outcomes": [
        [
          {
            "label": "Outcome",
            "type": "text",
            "field_name": "outcome",
            "value": "Outcome Data"
          },
          {
            "label": "ICD code",
            "type": "text",
            "field_name": "icd_code",
            "value": "ICD code Data"
          },
          {
            "label": "Symptoms",
            "type": "textarea",
            "field_name": "symptoms",
            "value": "Symptoms data"
          }
        ]
      ]
    },
    "id": "12364",
    "valid": null,
    "invalidFields": []
  },
  "message": [],
  "warnings": [],
  "errors": []
}
    </code>
  </div>

</div>

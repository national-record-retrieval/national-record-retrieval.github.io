<h1>get_timeline_request</h1>

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
      "example": 1,
    },
    "client_key": {
      "type": "string",
      "example": "key"
    },
    "request_type": {
      "type": "string",
      "example": "get_timeline_request"
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
  "request_type": "get_timeline_request",
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
  "type": "object",
  "properties": {
    "1697477959": {
      "type": "object",
      "description": "timeline message id"
      "properties": {
        "timestamp": {
          "type": "string",
          "example": 1697477959
        },
        "order_id": {
          "type": "string",
          "example": 735381
        },
        "event_type": {
          "type": "string",
          "example": "submit_order"
        },
        "submitted_at": {
          "type": "string",
          "example": "2023-10-16T13:39:18.000Z"
        },
        "submitted_at_date": {
          "type": "string",
          "example": "Mon 10/16/2023"
        },
        "submitted_at_time": {
          "type": "string",
          "example": "1:39 PM"
        },
        "patient": {
          "type": "string",
          "example": "Jane Doe"
        },
        "user": {
          "type": "string",
          "example": "Adylene Cruz"
        },
        "client_id": {
          "type": "string",
          "example": 1225
        },
        "client": {
          "type": "string",
          "example": "Keller Postman"
        },
        "provider": {
          "type": "string",
          "example": " "
        }
      }
    },
    "1697481680": {
      "type": "object",
      "description": "timeline message id",
      "properties": {
        "timestamp": {
          "type": "string",
          "example": 1697481680
        },
        "order_id": {
          "type": "string",
          "example": 735381
        },
        "event_type": {
          "type": "string",
          "example": "order_action"
        },
        "order_action": {
          "type": "string",
          "example": "verify"
        },
        "follow_up_days": {
          "type": "string",
          "example": null
        },
        "action_method": {
          "type": "string",
          "example": "web"
        },
        "action_date": {
          "type": "string",
          "example": "2023-10-16T14:41:15.000Z"
        },
        "comment_date": {
          "type": "string",
          "example": "Mon 10/16/2023"
        },
        "comment_time": {
          "type": "string",
          "example": "2:41 PM"
        },
        "comment": {
          "type": "string",
          "example": "Provider Memphis Children's Clinic - Memphis verified for order 735381"
        },
        "user": {
          "type": "string",
          "example": "AdminUser Role"
        },
        "email": {
          "type": "string",
          "example": "adminuser@nationalrr.com"
        },
        "client": {
          "type": "string",
          "example": "National Record Retrieval"
        },
        "provider_name": {
          "type": "string",
          "example": "Memphis Children's Clinic - Memphis"
        },
        "patient": {
          "type": "string",
          "example": "Jane Doe"
        }
      }
    },
    "1697481706": {
      "type": "object",
      "description": "timeline message id",
      "properties": {
        "timestamp": {
          "type": "string",
          "example": 1697481706
        },
        "event_type": {
          "type": "string",
          "example": "Document Received"
        },
        "file_name": {
          "type": "string",
          "example": "Test medical Records.pdf"
        },
        "user": {
          "type": "string",
          "example": "AdminUser Role"
        },
        "client_id": {
          "type": "string",
          "example": 1
        },
        "client": {
          "type": "string",
          "example": "National Record Retrieval"
        },
        "provider": {
          "type": "string",
          "example": "Memphis Children's Clinic - Memphis"
        }
      }
    },
    "1697481712": {
      "type": "object",
      "description": "timeline message id",
      "properties": {
        "timestamp": {
          "type": "string",
          "example": 1697481712
        },
        "order_id": {
          "type": "string",
          "example": 735381
        },
        "event_type": {
          "type": "string",
          "example": "order_action"
        },
        "order_action": {
          "type": "string",
          "example": "Complete"
        },
        "follow_up_days": {
          "type": "string",
          "example": 0
        },
        "action_method": {
          "type": "string",
          "example": "order"
        },
        "action_date": {
          "type": "string",
          "example": "2023-10-16T14:41:52.000Z"
        },
        "comment_date": {
          "type": "string",
          "example": "Mon 10/16/2023"
        },
        "comment_time": {
          "type": "string",
          "example": "2:42 PM"
        },
        "comment": {
          "type": "string",
          "example": null
        },
        "user": {
          "type": "string",
          "example": "AdminUser Role"
        },
        "email": {
          "type": "string",
          "example": "adminuser@nationalrr.com"
        },
        "client": {
          "type": "string",
          "example": "National Record Retrieval"
        },
        "provider_name": {
          "type": "string",
          "example": "Memphis Children's Clinic - Memphis"
        },
        "patient": {
          "type": "string",
          "example": "Jane Doe"
        },
        "subject": {
          "type": "string",
          "example": "AdminUser Role completed order for provider Memphis Children's Clinic - Memphis by order indicating that all record for patient Jane Doe were received. Order 735381 will remain active until all provider orders are marked complete."
        }
      }
    }
  }
}
    </code>

  </div>

  <div class='api_response'>
    <code>
{
  "1697477959": {
    "timestamp": "1697477959",
    "order_id": "735381",
    "event_type": "submit_order",
    "submitted_at": "2023-10-16 13:39:18",
    "submitted_at_date": "Mon 10/16/2023",
    "submitted_at_time": "1:39 PM",
    "patient": "Jane Doe",
    "user": "Adylene Cruz",
    "client_id": "1225",
    "client": "Keller Postman",
    "provider": "Memphis Children's Clinic - Memphis"
  },
  "1697481680": {
    "timestamp": "1697481680",
    "order_id": "735381",
    "event_type": "order_action",
    "order_action": "verify",
    "follow_up_days": null,
    "action_method": "web",
    "action_date": "2023-10-16 14:41:15",
    "comment_date": "Mon 10/16/2023",
    "comment_time": "2:41 PM",
    "comment": "Provider Memphis Children's Clinic - Memphis verified for order 735381",
    "user": "AdminUser Role",
    "email": "adminuser@nationalrr.com",
    "client": "National Record Retrieval",
    "provider_name": "Memphis Children's Clinic - Memphis",
    "patient": "Jane Doe"
  },
  "1697481706": {
    "timestamp": "1697481706",
    "event_type": "Document Received",
    "file_name": "Test medical Records.pdf",
    "user": "AdminUser Role",
    "client_id": "1",
    "client": "National Record Retrieval",
    "provider": "Memphis Children's Clinic - Memphis"
  },
  "1697481712": {
    "timestamp": "1697481712",
    "order_id": "735381",
    "event_type": "order_action",
    "order_action": "Complete",
    "follow_up_days": "0",
    "action_method": "order",
    "action_date": "2023-10-16 14:41:52",
    "comment_date": "Mon 10/16/2023",
    "comment_time": "2:42 PM",
    "comment": null,
    "user": "AdminUser Role",
    "email": "adminuser@nationalrr.com",
    "client": "National Record Retrieval",
    "provider_name": "Memphis Children's Clinic - Memphis",
    "patient": "Jane Doe",
    "subject": "AdminUser Role completed order for provider Memphis Children's Clinic - Memphis by order indicating that all record for patient Jane Doe were received. Order 735381 will remain active until all provider orders are marked complete."
  }
}
    </code>
  </div>

</div>

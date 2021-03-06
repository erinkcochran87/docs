---
tap: "netsuite-suite-analytics"
version: "1"
key: "event"

name: "events1"
doc-link: "https://www.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2020_1/odbc/record/calendarevent.html"
description: |
  {{ integration.append-only-loading | flatify }}

replication-method: "Key-based Incremental"
loading-behavior: "Append-Only"

attributes:
  - name: "date_last_modified"
    type: "date-time"
    replication-key: true
    description: |
      The time the {{ table.key | replace: "-"," " }} was last modified.

  - name: "access_level"
    type: "string"
    description: ""
  - name: "company_id"
    type: "integer"
    description: ""
  - name: "contact_id"
    type: "integer"
    description: ""
  - name: "date_0"
    type: "date-time"
    description: ""
  - name: "date_created"
    type: "date-time"
    description: ""
  - name: "event_extid"
    type: "string"
    description: ""
  - name: "event_id"
    type: "integer"
    description: ""
  - name: "is_timed_event"
    type: "string"
    description: ""
  - name: "location_0"
    type: "string"
    description: ""
  - name: "message"
    type: "string"
    description: ""
  - name: "opportunity_id"
    type: "integer"
    description: ""
  - name: "organizer_id"
    type: "integer"
    description: ""
  - name: "status"
    type: "string"
    description: ""
  - name: "supportcase_id"
    type: "integer"
    description: ""
  - name: "title"
    type: "string"
    description: ""
---
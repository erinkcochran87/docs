---
tap: "netsuite-suite-analytics"
version: "1"
key: "expense-amortization-rule"

name: "expense_amortization_rules"
doc-link: "https://www.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2020_1/odbc/record/expense_amortization_rules.html"
description: ""

replication-method: "Key-based Incremental"

attributes:
  - name: "{{ system-column.record-hash }}"
    type: "string"
    primary-key: true
    description: |
      {{ system-column.record-hash-netsuite-suite-analytics }}

      {{ integration.netsuite-primary-keys | flatify }}

  - name: "date_last_modified"
    type: "date-time"
    replication-key: true
    description: |
      The time the {{ table.key | replace: "-"," " }} was last modified.

  - name: "amount_source"
    type: "string"
    description: ""

  - name: "contra_account_id"
    type: "integer"
    description: ""
    foreign-key-id: "account-id"

  - name: "date_created"
    type: "date-time"
    description: ""

  - name: "end_date_change_impact"
    type: "string"
    description: ""

  - name: "end_date_source"
    type: "string"
    description: ""

  - name: "expense_rule_id"
    type: "integer"
    netsuite-primary-key: true
    description: ""
    foreign-key-id: "expense-rule-id"

  - name: "initial_amount"
    type: "string"
    description: ""

  - name: "name"
    type: "string"
    description: ""

  - name: "period_offset"
    type: "integer"
    description: ""

  - name: "recognition_period"
    type: "integer"
    description: ""

  - name: "reforecast_method"
    type: "string"
    description: ""

  - name: "residual"
    type: "string"
    description: ""

  - name: "rule_method"
    type: "string"
    description: ""

  - name: "start_date_source"
    type: "string"
    description: ""

  - name: "start_offset"
    type: "integer"
    description: ""

  - name: "term_in_days"
    type: "integer"
    description: ""

  - name: "term_in_months"
    type: "integer"
    description: ""
---
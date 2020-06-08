---
tap: "netsuite-suite-analytics"
version: "1"
key: "company"

name: "companies"
doc-link: "https://www.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2020_1/odbc/record/companies.html"
description: |
  {{ integration.netsuite-replication-keys | flatify }}

  {{ integration.append-only-loading | flatify }}

replication-method: "Key-based Incremental"

attributes:
  - name: "date_last_modified"
    type: "date-time"
    replication-key: true
    description: |
      The time the {{ table.key | replace: "-"," " }} was last modified.

  - name: "last_modified_date"
    type: "date-time"
    replication-key: true
    description: |
      The time the {{ table.key | replace: "-"," " }} was last modified.

  - name: "address"
    type: "string"
    description: ""

  - name: "address1"
    type: "string"
    description: ""

  - name: "address2"
    type: "string"
    description: ""

  - name: "address3"
    type: "string"
    description: ""

  - name: "city"
    type: "string"
    description: ""

  - name: "comments"
    type: "string"
    description: ""

  - name: "company_extid"
    type: "string"
    description: ""

  - name: "company_id"
    type: "integer"
    description: ""

  - name: "companyname"
    type: "string"
    description: ""

  - name: "country"
    type: "string"
    description: ""

  - name: "create_date"
    type: "date-time"
    description: ""

  - name: "currency_id"
    type: "integer"
    description: ""
    foreign-key-id: "currency-id"

  - name: "email"
    type: "string"
    description: ""

  - name: "full_name"
    type: "string"
    description: ""

  - name: "isinactive"
    type: "string"
    description: ""

  - name: "last_sales_activity"
    type: "date-time"
    description: ""

  - name: "loginaccess"
    type: "string"
    description: ""

  - name: "lsa_link"
    type: "string"
    description: ""

  - name: "lsa_link_name"
    type: "string"
    description: ""

  - name: "name"
    type: "string"
    description: ""

  - name: "parent_id"
    type: "integer"
    description: ""

  - name: "phone"
    type: "string"
    description: ""

  - name: "state"
    type: "string"
    description: ""

  - name: "stitch_custom_field"
    type: "number"
    description: ""

  - name: "stitch_custom_field_check_box"
    type: "string"
    description: ""

  - name: "stitch_custom_field_currency"
    type: "number"
    description: ""

  - name: "stitch_custom_field_decimal"
    type: "number"
    description: ""

  - name: "subsidiary"
    type: "integer"
    description: ""
    foreign-key-id: "subsidiary-id"

  - name: "url"
    type: "string"
    description: ""

  - name: "zipcode"
    type: "string"
    description: ""
---
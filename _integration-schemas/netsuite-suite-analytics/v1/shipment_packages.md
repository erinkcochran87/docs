---
tap: "netsuite-suite-analytics"
version: "1"
key: "shipment-package"

name: "shipment_packages"
doc-link: "https://www.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2020_1/odbc/record/shipment_packages.html"
description: ""

replication-method: "Full Table"

attributes:
  - name: "admissibility_package_type"
    type: "string"
    description: ""
  - name: "alcohol_recipient_type"
    type: "string"
    description: ""
  - name: "authorization_number"
    type: "string"
    description: ""
  - name: "carrier_packaging"
    type: "string"
    description: ""
  - name: "cash_on_delivery_amount"
    type: "integer"
    description: ""
  - name: "cash_on_delivery_method"
    type: "string"
    description: ""
  - name: "cod_other_charge"
    type: "integer"
    description: ""
  - name: "contents_description"
    type: "string"
    description: ""
  - name: "declared_value"
    type: "integer"
    description: ""
  - name: "delivery_confirmation"
    type: "string"
    description: ""
  - name: "dimension_unit"
    type: "string"
    description: ""
  - name: "dry_ice_weight"
    type: "integer"
    description: ""
  - name: "freight_charge_added_to_cod"
    type: "string"
    description: ""
  - name: "has_additional_handling"
    type: "string"
    description: ""
  - name: "has_cash_on_delivery"
    type: "string"
    description: ""
  - name: "has_declared_value"
    type: "string"
    description: ""
  - name: "has_insured_value"
    type: "string"
    description: ""
  - name: "insured_value"
    type: "integer"
    description: ""
  - name: "is_alcohol"
    type: "string"
    description: ""
  - name: "is_non_hazardous_li_batteries"
    type: "string"
    description: ""
  - name: "is_non_standard_container"
    type: "string"
    description: ""
  - name: "item_fulfillment_id"
    type: "integer"
    description: ""
  - name: "package_height"
    type: "integer"
    description: ""
  - name: "package_length"
    type: "integer"
    description: ""
  - name: "package_width"
    type: "integer"
    description: ""
  - name: "priority_alert_content"
    type: "string"
    description: ""
  - name: "priority_alert_type"
    type: "string"
    description: ""
  - name: "reference_one"
    type: "string"
    description: ""
  - name: "reference_two"
    type: "string"
    description: ""
  - name: "signature_option"
    type: "string"
    description: ""
  - name: "signature_release"
    type: "string"
    description: ""
  - name: "tracking_number"
    type: "string"
    description: ""
  - name: "weight_in_lbs"
    type: "integer"
    description: ""
  - name: "your_packaging"
    type: "string"
    description: ""
---
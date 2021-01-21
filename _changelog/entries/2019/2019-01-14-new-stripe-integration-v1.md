---
title: New version (v1) of Stripe integration
content-type: "changelog-entry"
date: 2019-01-14
entry-type: new-feature
entry-category: integration
connection-id: stripe
connection-version: 1
---
{{ site.data.changelog.metadata.single-integration | flatify }}

A new version (v{{ integration.this-version }}) of our {{ integration.display_name }} integration is now available! 

We’ve worked hard to ensure this new integration is the best way to extract data from {{ integration.display_name }} to your Stitch destination. The new integration, based on the [Singer standard]({{ site.singer }}){:target="new"}, includes many new features such as:

- Removal of `stripe_` prefixes from table names
- New and improved tables, including:
  - [invoice_line_items]({{ this-connection.url | prepend: site.baseurl | append: "#invoice_line_items" }})
  - [subscription_items]({{ this-connection.url | prepend: site.baseurl | append: "#subscription_items" }})
  - [subscription_line_items]({{ this-connection.url | prepend: site.baseurl | append: "#subscription_line_items" }})
  - The `transfer_transactions` table has been replaced by [payouts]({{ this-connection.url | prepend: site.baseurl | append: "#payouts" }})
- User-facing [Extraction Logs]({{ link.replication.extraction-logs | prepend: site.baseurl }})
- [Table and field selection]({{ link.replication.syncing | prepend: site.baseurl }})
- Availability via the [Stitch Connect API]({{ link.connect.overview | prepend: site.baseurl }})

Get started today by creating a new {{ this-connection.display_name }} integration or learn more in the [updated documentation]({{ this-connection.url | prepend: site.baseurl }}).
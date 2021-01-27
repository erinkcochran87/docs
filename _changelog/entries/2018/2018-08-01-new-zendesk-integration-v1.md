---
title: New version (v1) of Zendesk integration
content-type: "changelog-entry"
date: 2018-08-01
entry-type: new-feature
entry-category: integration
connection-id: zendesk
connection-version: 1
---
{{ site.data.changelog.metadata.single-integration | flatify }}

A new version (v{{ this-connection.this-version }}) of our {{ this-connection.display_name }} integration is now available! 

We’ve worked hard to ensure this new integration is the best way to extract data from {{ this-connection.display_name }} to your Stitch destination. The new integration, based on the [Singer standard]({{ site.singer }}){:target="new"}, includes many new features such as:

- User-facing [Extraction Logs]({{ link.replication.extraction-logs | prepend: site.baseurl }})
- [Table and field selection]({{ link.replication.syncing | prepend: site.baseurl }})
- [Run and stop Extraction]({{ link.replication.start-stop-extraction | prepend: site.baseurl }}) on demand functionality
- Availability via the [Stitch Connect API]({{ link.connect.overview | prepend: site.baseurl }})
- Enhanced schema validation

Get started today by creating a new {{ this-connection.display_name }} integration or learn more in the [updated documentation]({{ this-connection.url | prepend: site.baseurl }}).
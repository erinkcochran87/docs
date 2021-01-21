---
title: New version (v1) of Microsoft SQL Server integration
content-type: "changelog-entry"
date: 2019-07-15
entry-type: new-feature
entry-category: integration
connection-id: "mssql"
connection-version: 1
---
{{ site.data.changelog.metadata.single-integration | flatify }}

A new version (v{{ integration.this-version }}) of our {{ integration.display_name }} integration is now available! 

We’ve worked hard to ensure this new integration is the best way to extract data from {{ integration.display_name }} databases to your Stitch destination. The new integration, based on the [Singer standard]({{ site.singer }}){:target="new"}, includes many new features such as:

- [Logical Replication]({{ link.replication.log-based-incremental | prepend: site.baseurl }}) support via SQL Server Change Tracking
- User-facing [Extraction Logs]({{ link.replication.extraction-logs | prepend: site.baseurl }})
- [Enhanced scheduling options]({{ link.replication.rep-scheduling | prepend: site.baseurl }})
- [Run and stop Extraction]({{ link.replication.start-stop-extraction | prepend: site.baseurl }}) on demand functionality
- Availability via the [Stitch Connect API]({{ link.connect.overview | prepend: site.baseurl }})

Get started today by creating a new {{ integration.display_name }} integration or learn more in the [updated documentation]({{ integration.url | prepend: site.baseurl }}).
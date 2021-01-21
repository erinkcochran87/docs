---
title: New version (v1) of NetSuite integration
content-type: "changelog-entry"
date: 2019-05-16
entry-type: new-feature
entry-category: integration
connection-id: netsuite
connection-version: 1
---
{{ site.data.changelog.metadata.single-integration | flatify }}

A new version (v{{ integration.this-version }}) of our {{ integration.display_name }} integration is now available! 

We’ve worked hard to ensure this new integration is the best way to extract data from {{ integration.display_name }} to your Stitch destination. The new integration, based on the [Singer standard]({{ site.singer }}){:target="new"}, includes many new features such as:

- Removal of `netsuite_` prefixes from table names
- {{ integration.display_name }} token based authentication
- Optimizations to API concurrency during discovery of tables/fields
- Utilization of an updated {{ integration.display_name }} WSDL for a more complete set of tables/fields
- [Field selection]({{ link.replication.syncing | prepend: site.baseurl }})

Get started today by creating a new {{ integration.display_name }} integration or learn more in the [updated documentation]({{ integration.url | prepend: site.baseurl }}).
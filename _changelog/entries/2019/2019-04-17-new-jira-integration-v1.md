---
title: New version (v1) of JIRA integration
content-type: "changelog-entry"
date: 2019-04-17
entry-type: new-feature
entry-category: integration
connection-id: jira
connection-version: 1
---
{{ site.data.changelog.metadata.single-integration | flatify }}

A new version (v{{ integration.this-version }}) of our {{ integration.display_name }} integration is now available! 

We’ve worked hard to ensure this new integration is the best way to extract data from {{ integration.display_name }} to your Stitch destination. The new integration, based on the [Singer standard]({{ site.singer }}){:target="new"}, includes many new features such as:

- Removal of `jira_` prefixes from table names
- New tables, including:
  - [issues]({{ integration.url | prepend: site.baseurl | append: "#issues" }}), [changelog]({{ integration.url | prepend: site.baseurl | append: "#changelog" }}), and [transitions]({{ integration.url | prepend: site.baseurl | append: "#transitions" }}) are now top-level tables
  - [roles]({{ integration.url | prepend: site.baseurl | append: "#worklogs" }}) (formerly `jira_project_roles`)
  - [worklogs]({{ integration.url | prepend: site.baseurl | append: "#worklogs" }})
- {{ integration.display_name }} Cloud accounts now use an API token instead of user/password authentication
- User-facing [Extraction Logs]({{ link.replication.extraction-logs | prepend: site.baseurl }})
- [Table and field selection]({{ link.replication.syncing | prepend: site.baseurl }})
- [Run and stop Extraction]({{ link.replication.start-stop-extraction | prepend: site.baseurl }}) on demand functionality
- Enhanced schema validation

Get started today by creating a new {{ integration.display_name }} integration or learn more in the [updated documentation]({{ integration.url | prepend: site.baseurl }}).
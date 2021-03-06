---
tap-reference: "asana"

version: "2"

foreign-keys:
  - id: "project-id"
    attribute: "gid"
    table: "projects"
    all-foreign-keys:
      - table: "projects"
      - table: "tasks"
        subtable: "projects"
      - table: "stories"
        subtable: "projects"
      - table: "sections"
        subtable: "project"
      - table: "sections"
        subtable: "projects"     

  - id: "tag-id"
    attribute: "gid"
    table: "tags"
    all-foreign-keys:
      - table: "tags"
      - table: "stories"
        subtable: "tag"

  - id: "task-id"
    attribute: "gid"
    table: "tasks"
    all-foreign-keys:
      - table: "tasks"
      - table: "stories"
        subtable: "task"

  - id: "user-id"
    attribute: "gid"
    table: "users"
    all-foreign-keys:
      - table: "projects"
        subtable: "followers"
      - table: "projects"
        subtable: "members"
      - table: "projects"
        subtable: "owner"
      - table: "tags"
        subtable: "followers"
      - table: "tasks"
        subtable: "assignees"
      - table: "tasks"
        subtable: "followers"
      - table: "users"
      - table: "stories"
        subtable: "assignees"
      - table: "stories"
        subtable: "created_by"
      - table: "stories"
        subtable: "dependency"
      - table: "portfolios"
        subtable: "created_by"
      - table: "portfolios"
        subtable: "members" 
      - table: "porfolios"
        subtable: "owner" 
      - table: "teams"
        subtable: "users"     


  - id: "workspace-id"
    attribute: "gid"
    table: "workspace"
    all-foreign-keys:
      - table: "projects"
        subtable: "workspace"
      - table: "tags"
        subtable: "workspace"
      - table: "tasks"
        subtable: "workspace"
      - table: "users"
        subtable: "workspace"
      - table: "workspace"
      - table: "portfolios"
        subtable: "workspace"
      - table: "teams"
        subtable: "organization"  

  - id: "section-id"
    attribute: "gid"
    table: "sections"
    all-foreign-keys:
      - table: "sections"
      - table: "stories"
        subtable: "new_section"
      - table: "stories"
        subtable: "old_section"

  - id: "story-id"
    attribute: "gid"
    table: "stories"
    all-foreign-keys:
      - table: "stories"
      - table: "stories"
        subtable: "story"

  - id: "portfolio-id"
    attribute: "gid"
    table: "porfolios"
    all-foreign-keys:
      - table: "portfolios"
      - table: "portfolios"  
        subtable: "portfolio_items"              
---
---
page_title: "looker_project Data Source - terraform-provider-looker"
subcategory: ""
description: |-
  
---
# looker_project (Data Source)

## Example Usage
```terraform
data "looker_project" "project" {
    name = "project-a"
}
```
## Example Output
```terraform
# looker_project.project:
resource "looker_project" "project" {
  rename_when_delete = true
  id                 = "project-a-AgcX"
  name               = "project-a"
}
```
<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) Porject name

### Read-Only

- `allow_warnings` (Boolean) Validation policy: If true, the project can be committed with warnings when
- `git_remote_url` (String) Git remote repository url.
- `git_service_name` (String) Name of the git service provider.
- `git_username` (String) Git username for HTTPS authentication.
- `id` (String) The ID of this resource.
- `is_example` (Boolean) If true, the project is an example project and cannot be modified.
- `uses_git` (Boolean) If true, the project uses a git repository.
- `validation_required` (Boolean) Validation policy: If true, the project must pass validation checks before project changes can be committed to the git repository

---
page_title: "looker_folder Data Source - terraform-provider-looker"
subcategory: ""
description: |-
  
---
# looker_folder (Data Source)

## Example Usage
```terraform
resource "looker_folder" "folder" {
  id = "123"
}
```
## Example Output
```terraform
# looker_folder.folder:
resource "looker_folder" "folder" {
  id   = "123"
  name = "USA"
}
```
<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `id` (String) Search folder based on id.
- `name` (String) Search folder based on name.

### Read-Only

- `parent_id` (String) Id of the parent folder.

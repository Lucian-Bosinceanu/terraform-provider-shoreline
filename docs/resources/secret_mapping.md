---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "shoreline_secret_mapping Resource - terraform-provider-shoreline"
subcategory: ""
description: |-
  Shoreline secret_mapping. A mapping associated with a secret available in Shoreline and usable within the context of a runbook.
---

# shoreline_secret_mapping (Resource)

Shoreline secret_mapping. A mapping associated with a secret available in Shoreline and usable within the context of a runbook.



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **name** (String) The name/symbol for the object within Shoreline and the op language (must be unique, only alphanumeric/underscore).
- **public_alias** (String) The name used to reference the secret in the runbook's parameters.

### Optional

- **namespace** (String) Applicable only to remotely managed secrets. Defines the namespace where the secret is available.
- **path** (String) Applicable only to remotely managed secrets. Specifies the path to the remote secret.
- **secret_name** (String) The name of the existing secret linked to the mapping.

### Read-Only

- **id** (String) The ID of this resource.
- **type** (String) The type of object (i.e., Alarm, Action, Bot, Metric, Resource, or File).
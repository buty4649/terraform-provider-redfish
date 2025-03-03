---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "redfish_virtual_media Resource - terraform-provider-redfish"
subcategory: ""
description: |-
  
---

# redfish_virtual_media (Resource)





<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `image` (String) The URI of the remote media to attach to the virtual media
- `redfish_server` (Block List, Min: 1) List of server BMCs and their respective user credentials (see [below for nested schema](#nestedblock--redfish_server))
- `virtual_media_id` (String) ID from the virtual media to be used. I.E: RemovableDisk

### Optional

- `inserted` (Boolean) The URI of the remote media to attach to the virtual media
- `password` (String) The password to access the image parameter-specific URI
- `transfer_method` (String)
- `transfer_protocol_type` (String)
- `username` (String) The username to access the image parameter-specific URI
- `write_protected` (Boolean)

### Read-Only

- `id` (String) The ID of this resource.

<a id="nestedblock--redfish_server"></a>
### Nested Schema for `redfish_server`

Required:

- `endpoint` (String) Server BMC IP address or hostname

Optional:

- `password` (String, Sensitive) User password for login
- `ssl_insecure` (Boolean) This field indicates whether the SSL/TLS certificate must be verified or not
- `user` (String) User name for login



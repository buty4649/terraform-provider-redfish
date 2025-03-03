---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "redfish_power Resource - terraform-provider-redfish"
subcategory: ""
description: |-
  
---

# redfish_power (Resource)





<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `check_interval` (Number) The frequency with which to check the server's power state in seconds
- `desired_power_action` (String) Desired power setting. Applicable values 'On','ForceOn','ForceOff','ForceRestart','GracefulRestart','GracefulShutdown','PowerCycle'
- `maximum_wait_time` (Number) The maximum amount of time to wait for the server to enter the correct power state beforegiving up in seconds
- `redfish_server` (Block List, Min: 1) List of server BMCs and their respective user credentials (see [below for nested schema](#nestedblock--redfish_server))

### Read-Only

- `id` (String) The ID of this resource.
- `power_state` (String) Desired power setting. Applicable values 'On','ForceOn','ForceOff','ForceRestart','GracefulRestart','GracefulShutdown','PowerCycle'.

<a id="nestedblock--redfish_server"></a>
### Nested Schema for `redfish_server`

Required:

- `endpoint` (String) Server BMC IP address or hostname

Optional:

- `password` (String, Sensitive) User password for login
- `ssl_insecure` (Boolean) This field indicates whether the SSL/TLS certificate must be verified or not
- `user` (String) User name for login



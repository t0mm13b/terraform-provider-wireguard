---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "wireguard_preshared_key Resource - terraform-provider-wireguard"
subcategory: ""
description: |-
  Provides a WireGuard key resource. This can be used to create, read, and delete WireGuard preshared keys in terraform state.
---

# wireguard_preshared_key (Resource)

Provides a WireGuard key resource. This can be used to create, read, and delete WireGuard preshared keys in terraform state.

## Example Usage

```terraform
resource "wireguard_preshared_key" "example" {
}

output "wg_preshared_key" {
  description = "Example's preshared WireGuard key"
  value       = wireguard_preshared_key.example.key
  sensitive   = true
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `id` (String) The ID of this resource.

### Read-Only

- `key` (String, Sensitive) Additional layer of symmetric-key cryptography to be mixed into the already existing public-key cryptography, for post-quantum resistance.



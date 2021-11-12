---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "grafana_synthetic_monitoring_probe Data Source - terraform-provider-grafana"
subcategory: ""
description: |-
  Data source for retrieving a single probe by name.
---

# grafana_synthetic_monitoring_probe (Data Source)

Data source for retrieving a single probe by name.

## Example Usage

```terraform
data "grafana_synthetic_monitoring_probe" "atlanta" {
  name = "Atlanta"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **name** (String) Name of the probe.

### Read-Only

- **id** (String) The ID of the probe.
- **labels** (Map of String) Custom labels to be included with collected metrics and logs.
- **latitude** (Number) Latitude coordinates.
- **longitude** (Number) Longitude coordinates.
- **public** (Boolean) Public probes are run by Grafana Labs and can be used by all users. Only Grafana Labs managed public probes will be set to `true`.
- **region** (String) Region of the probe.
- **tenant_id** (Number) The tenant ID of the probe.


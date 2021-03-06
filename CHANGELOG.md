## 1.1.1 (Unreleased)

## 1.1.0 (March 10, 2020)

FEATURES:

* **New Resource:** `vmc_sddc`
* **New Resource:** `vmc_public_ip` [\#43](https://github.com/vmware/terraform-provider-vmc/pull/43)
* **New Data Source:** `vmc_org`
* **New Data Source:** `vmc_connected_accounts`
* **New Data Source:** `vmc_customer_subnets`


ENHANCEMENTS:

* vmc_sddc: Added nsxt_reverse_proxy_url to SDDC resource data. [\#23](https://github.com/vmware/terraform-provider-vmc/pull/23)
* vmc_connected_accounts: Added filtering to return AWS account ID associated with the account number provided in configuration. [\#30](https://github.com/vmware/terraform-provider-vmc/pull/30)
* provider.go: Added org_id as a required parameter in terraform schema. [\#38](https://github.com/vmware/terraform-provider-vmc/pull/38)
* data_source_vmc_customer_subnets.go : Added validateFunctions for sddc and customer subnet resources. [\#41](https://github.com/vmware/terraform-provider-vmc/pull/41)
* examples/main.tf : Added expression to convert AWS specific region to VMC region. [\#46](https://github.com/vmware/terraform-provider-vmc/pull/46) 


BUG FIXES:

* Moved main.tf to examples folder. [\#17](https://github.com/vmware/terraform-provider-vmc/pull/17)
* License statement fixed. [\#8](https://github.com/vmware/terraform-provider-vmc/pull/8)
* Implemented connected account data source to return a single account ID associated with the account number. [\#40](https://github.com/vmware/terraform-provider-vmc/pull/40)
* Set ForceNew for host_instance_type to true in order to enforce SDDC redeploy when host_instance_type is changed. [\#5](https://github.com/terraform-providers/terraform-provider-vmc/pull/5)

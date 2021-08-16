
## Azure Infrastructure code for Snowflake

IaC to deploy necessary pieces for a landing zone to input data from On-prem up into Azure.  Leveraging Terraform here for ease of use. The key pieces of infrastructure to host Snowflake are:
- Azure KeyVault 
- Azure Storage Account (with ADLSgen2 enabled)
- Azure PrivateDNS Zone (for use with privatelink)
- DNS Server VM
- Matillion VM (from Marketplace ETL)
- HVR VM (large enough for HVR Hub and Postgresql DB)
- Workstation VM (multiuser for devs)
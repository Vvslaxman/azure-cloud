# azure-cloud

## Cloud Deployment Model
Cloud Deployment Model is simple a separation which describes where are the company resources deployed. Whenever this is in public cloud provider environment or private datacenter.

Layer  |	Cloud Provider | Own Datacenter
Public |	✅	           |    ✖
Hybrid |	✅             |   ✅
Private|	✖              |	  ✅
## Public Cloud
### Key Characteristics

- Everything runs on cloud provider hardware
- No local hardware
- Some services share hardware with other customers
### Advantages

- No CapEx (No initial investment)
- High Availability
- Agility
- Pay as you Go (PAYG) pricing
- No hardware maintenance
- No deep technical skills required
### Disadvantages

- Not all security and compliance policies can be met
- No ownership over the physical infrastructure
- Rare specific scenarios can’t be done
## Private Cloud
### Key Characteristics

- Everything runs on your own datacenter
- Self-service should be provided
- You maintain the hardware
### Advantages

- Can support any scenario
- Total control over security and infrastructure
- Can meet any security and compliance policy
### Disadvantages

- Initial investment is required (CapEx)
- Limited agility constrained by server capacity and team skills
- Very dependent on IT skills & expertise

## Hybrid Cloud
### Key Characteristics

- Combines both Public & Private cloud
### Advantages

- Great flexibility
- You can run any legacy apps in private cloud
- Can utilize existing infrastructure
- Meet any security& compliance requirements
- Can take advantage of all public cloud benefits
### Disadvantages

- Can be more expensive
- Complicated to manage due to larger landscape
- Most dependent on IT skills & expertise from all three models

## Data Center
- Physical facility
- Hosting for group of networked servers
- Own power, cooling & networking infrastructure
## Region
- Geographical area on the planet
- One but usually more datacenters connected with low-latency network (<2 milliseconds)
- Location for your services
- Some services are available only in certain regions
- Some services are global services, as such are not assigned/deployed in specific region
- Globally available with 50+ regions
- Special government regions (US DoD Central, US Gov Virginia, etc.)
- Special partnered regions (China East, China North)
## Availability Zone
- Regional feature
- Logical grouping of physically separate facilities that have their own independent cooling, power and networking infrastructure
- Designed to protect from data center failures
- If zone goes down others continue working
- Two service categories
1. Zonal services (Virtual Machines, Disks, etc.)<-> Create a VM-> Availability options-> Availability zones/Availability set -> Availability zone-> 1/2/3
2. Zone-redundant services (SQL, Storage, etc.)<-> Create storage accound->Replication->ZR Storage
- Not all regions are supported
- Supported region has three or more zones(>=3)
- A zone is one or more data centers
## Region Pair
- Each region is paired with another region making it a region pair
- Region pairs are static and cannot be chosen
- Each pair resides within the same geography*
- Exception is Brazil South
- Physical isolation with at least 300 miles distance (when possible)
- Some services have platform-provided replication
- Planned updates across the pairs are synchronized to ensure that they are not updated at the same time
- Data residency maintained for disaster recovery
- Region Pair A	-> Region Pair B
1. East US		-> West US
2. UK West		-> UK South
3. North Europe (Ireland)		-> West Europe (Netherlands)
4. East Asia (Hong Kong)	-> 	Southeast Asia (Singapore)
## Geographies
- Discrete market
- Typically contains two or more regions
- Ensures data residency, sovereignty, resiliency, and compliance requirements are met
- Fault tolerant to protect from region wide failures
- Broken up into areas like Americas, Europe, Asia Pacific, Middle East and Africa
- Each region belongs only to one Geography

## Azure Resource
- Object used to manage services in Azure
- Represents service lifecycle
- Saved as JSON definition
## Resource Groups
- Grouping of resources
- Holds logically related resources
- Typically organizing by
1.Type
2. Lifecycle (app, environment)
3. Department
4. Billing,
5. Resource type
6. Location or
7. combination of those
## Azure Resource Manager
- Management Layer for all resources and resource groups
- Unified language
- Controls access and resources
## Additional Info
- Each resource must be in one, and only one resource group
- Resource groups can contain resources from their own location assigned
- Resources in the resource groups can reside in a different locations
- Resources can be moved between the resource groups
- Most azure reasources can be moved to a different Azure subscription/resource group easily.
- A resource group assignement is required when creating any resource
- Resource groups can’t be nested
- Organize based on your organization needs but consider
1. Billing
2. Security and access management
3. Application Lifecycle
 
 

  

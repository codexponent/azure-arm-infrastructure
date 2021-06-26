# azure-arm
Azure ARM for Storage Account and Virutal Machine

# Motivation
Let's say we have an infrastructure in place. There may be a time that we need to replicate the same infrastructure again. Doing it manually will surely give us an error in the migration stages. So, we will be utilizing a service from Azure called Azure ARM Templates to deploy our infrastructure in an idempotent way.

# Architecture
![architecture](https://user-images.githubusercontent.com/13358738/123505467-f5068280-d67e-11eb-83d4-0c807db19402.png)


# Tools:
1. Azure Account
2. Azure Virtual Machines
3. Azure VNet
4. Azure Templates
5. Azure Storage Account

# Replication Steps

```bash
git clone git@github.com:codexponent/azure-arm-infrastructure.git
az create group --name prem-vm --location eastus
az deployment group create --resource-group prem-rg --template-file template.json
```

For the rest of the explanation and demonstration I have it on my medium blog.








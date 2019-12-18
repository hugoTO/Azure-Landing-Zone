# Azure Migration Landing Zone #

- Migration landing zone is a term used to describe an environment that has been provisioned and prepared to host workloads being migrated from an on-premises environment into Azure
- Migration landing zone is intentionally limited which is designed to create a consistent starting point that provides room to learn infrastructure as code
- Use the Cloud Adoption Framework migrate landing zone blueprint to deploy the defined environment with a minimal effort

## Table of content ##

1. Prerequisite
2. Create Blueprint
3. Add RDP Rule from Internet to Jumpbox Subnet
4. Create Virtual Machine
5. Encrypt Virtual Machines
6. Firewalls Configuration
7. Log Analytics Configuration
8. Security Center Configuration

## Prerequisite ##

### Azure subscription ###
A Azure subscription is required. If your organization already using Azure, please sign up a new Azure account with your personal email and use [Azure Pass](https://www.microsoftazurepass.com/) to redeem Azure Credit.

### PowerShell 5.1 with Az Module installed ###
1. Search and type ***PowerShell*** in search box and run Windows PowerShell as Administrator
2. Type ***$PSVersionTable.PSVersion*** and press enter
3. See if the version of the PowerShell is 5.1. If not, please go to [here])(https://docs.microsoft.com/en-us/powershell/scripting/install/installing-windows-powershell?view=powershell-6) to update your existing version of PowerShell to 5.1
4. Type ***Install-Module -Name -Az -AllowClobber -Scope AllUsers*** and press enter
5. Type ***Get-InstalledModule -Name -Az -AllVersions | select Name, Version*** and press enter to see if Az Module is installed

## Create Blueprint ##



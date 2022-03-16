# Windows Hello for Business Implementation
This repository holds all of my scripts and resources for implementing Windows Hello for Business into a lab environment for testing or educational purposes.

This lab is based on a [hybrid key trust deployment.](https://docs.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust)

The files prefixed with "Create-" create new resources in Azure using Azure PowerShell, these can be ignored if using on-premises machines such as VMWare ESXi or Workstation VMs. The files prefixed with "Deploy-" are specific to each machine (Domain Controller, Certificate Authority, Web Server) and are intended to be run from within each machines environment. If you decide to use these lab files for on-premises machines you will need to manually configure networking as I am automating this for Azure resources but not for on-premises machines.

## Machines
* Domain Controller (vm-adds01-aue)
* Certificate Authority (vm-ca01-aue)

## Requirements
* Azure Active Directory P1 or P2 license
* Internet connectivity on the DC for AAD Connect

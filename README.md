# active_directory

## 00 - Install VMs

1. Installed Windows Server 2022 as a Virtual machine in VMware Workstation Pro
2. Installed Windows 11 as a Virtual machine in VMware Workstation Pro

## 01 - Installing the Domain Controller

1. Use `sconfig` to:
    - Change the hostname
    - Change the IP address to static
    - Change the DNS server to our own IP address

2. Install the Active Directory Windows Feature

```shell
Install-WindowsFeature -name AD-Domain-Services -IncludeManagementTools
```
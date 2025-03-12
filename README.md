# Ubuntu-VM-Policy
`az policy definition create   --name "deny-vm-without-availability"   --display-name "Deny VM creation without availability options"   --description "This policy denies the creation of VMs that do not have an Availability Set or Availability Zone."   --rules https://ubuntupolicystorage.blob.core.windows.net/policycontainer/deny-vm-without-availability.json  --mode All`
`az policy assignment create --policy deny-vm-without-availability`
`az policy assignment list`
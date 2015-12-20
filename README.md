# virtualbox-setup
How to setup virtualbox on a current ubuntu machine running an ubuntu lts server

## Install virtualbox
- Use "Ubuntu 14.04" as name for the vm
- I decided to go for OpenSSH server only if asked

## Create a virtual network interface on the host system
(Source: https://www.virtualbox.org/manual/ch06.html#network_hostonly )
`VBoxManage hostonlyif create`

## Set up the second network adapter in order to access the vm ubuntu via ssh from host
(Source: https://www.virtualbox.org/manual/ch06.html#network_hostonly )
`VBoxManage modifyvm "Ubuntu 14.04" --nic2 hostonly`

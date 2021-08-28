<p align="center">
  <img src="./SSH_Logo.png"/>
</p>

<h1 align="center">0x00. SSH TOOLS</h1>
<p align="center"></p>
## Description
Some script in bash for tasks in ssh

## How to install it:
```
git clone https://github.com/Frank-Grijalba/SSH_TOOLS.git
cd SSH_TOOLS
```
### To keep in mind...
Before executing any of the following commands, it is important to take into account to create the "Alias" in our local computer which is configured in the file located in /etc/hosts but we make it easier using the file found in this repository called <br>setup_alias_ssh</br>.
It is important to configure the "Alias" since it will be used in the correct execution of all the files contained in this repository.

#### Commands Sintax with Respective Usage
File | Description | Usage
------- | ------ | ------
setup_alias_ssh | Configure the Alias of the server in the local machine |  `./setup_alias_ssh ALIAS USER IP SSH_KEY_PATH`
f_transfer_scp_fromserver | This file use the SCP command to transfer a file from the server to the local machine | `./f_transfer_scp_fromserver SSH_ALIAS FILE_FOLDER_FROM_SERVER LOCAL_FOLDER_TO_SAVE`
f_transfer_scp_toserver | This file use the SCP command to transfer a file to the server from the local machine | `./f_transfer_scp_toserver SSH_KEY_PATH LOCAL_FILE SSH_ALIAS FOLDER_ON_SERVER`
f_transfer_SFTP_TOserver | This file use the SFTP command to transfer a file to the server from the local machine | `./f_transfer_SFTP_ToServer SSH_KEY_PATH SSH_ALIAS`
file_transfer_rsync | This file use the RSYNC command to transfer a file to the server from the local machine without interruptions | `./file_transfer_rsync LOCAL_FILE SSH_ALIAS`
ssh_conn | Use this file to connect to the server | `./ssh_conn SSH-KEY-PATH SSH_ALIAS`
ssh_execute | Use this file to execute commands from the server, the command will be in quotes | `./ssh_execute SSH_ALIAS "COMMAND_TO_EXECUTE"`

### Other tool
File | Description | Usage
------- | ------ | ------
service_restart | Use this file to restart any service | `./service_restart SERVICE`

# Author

👤 **Frank J. Grijalba H.**

- Twitter: [@FrankGrijalba](https://twitter.com/FrankGrijalba)
- Github: [@FRANK-GRIJALBA](https://github.com/FRANK-GRIJALBA)

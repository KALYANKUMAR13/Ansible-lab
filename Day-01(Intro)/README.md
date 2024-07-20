System Admin (Before DevOps) - their role is configuration management.
There are 4 linux based servers and 1 windows server in a company
Their roles:
1. Each of linux based servers/windows should be up to date or all should have a same supported version.
2. Packages and libraries such as openssh/wget/curl. along with the cent os, package version should be same and supported version.
3. In case of Java  -> supported java version, webserver, application server. The 3 should be same version insalled in all systems.
4. Maintenance of servers, like cpu,
Shellscripting will not work in windows based server and in linux based servers, if the os is different like CentOS, ubuntu

To overcome above issues, configuration managements tools introduced like - Chef, Puppet, SaltStack and Ansible.

Chef and Puppet need more learning curve. and Need to have agent in all system/servers that need to work with them.

So finally Ansible came -> know the yamlfile(playbooks), it is agentless

Control Node - The machine on which we install Ansible software is called Control node. From control node, we can manage all manage nodes
Manage Nodes - The machines, in which we can install the software/package/libraries is called managenode. Manage node can be any Distribution

Ansible is Automation Platform 
Now  can perform:
1. Provisioning (like IaC terraform)
2. Configuration Management(core Feature)
3. CICD (Deploying the artifact to the target server) 
4. Network automation

Choosing script
Whenever we need to talk to APi or other platform like Jira, Gihub, we can go for python scripting.

In all both control and manage nodes, we need to have python installed. so anible able to manage all servers/
linux-ssh
windows -winrm 
Control node should be linux based one.

To install ansible in window, 
1. First install wsl, Open powershell in a admin mode and 
```
wsl --install
```
2. Update the pacakge list
```
sudo apt update
sudo apt upgrade
```
3. Add Ansible official PPA (Personal Package Archieve)
```
sudo apt-add-repository --yes --update ppa:ansible/ansible
```
4. Install ansible 
```
sudo apt install ansible
```

Finally, check the version that is installed,
```
ansible --version
```

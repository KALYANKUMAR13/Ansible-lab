Yaml file(playbook) or we can use command i.e Adhoc command

PasswordLess Authentication

1. password for the first time
2. ssh for the first time

Attaching(adding) the public key in particular VM is a method of ssh less authentication.

If you are using, aws ec2:
```
ssh-copy-id -f "-o IdentityFile <PATH TO PEM FILE>" ubuntu@<INSTANCE-PUBLIC-IP>
```
```
 ssh <USERNAME OF THE KEY>@<EXTERNAL-IP>
```
----------------------------------------------------
For password,
Go to particular file 
```
sudo vim /etc/ssh/sshd_config.d/60-cloudimg-settings.conf
sudo systemctl restart ssh
```
Update PasswordAuthentication yes

Then, create a password the particular user, here ubuntu
```
sudo passwd ubuntu
```
-----------------------------------------------------------------
Inventory
1. Inventory.ini file
2. yaml file

The file can be anywhere but need to pass while we are execting  OR go to /etc/ansible/hosts , we need to to specify the username and ip here.
the ini or yaml file is recommended.

2 ways 
1. ad-hoc
2. yaml files(playbook)

playbooks are reuseable, share , versioncontrol by uploading to git
adhoc command
```
 ansible -i inventory.ini -m "shell" -a "ls -la" all
```
-m module
-a argument

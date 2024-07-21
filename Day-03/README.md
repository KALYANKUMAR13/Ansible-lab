Get the yaml file,

Update the inventory.ini, if you are not using static IP.

Be in the directory, where play is there.
```
ansible-playbook -i <InventoryFileLocationandFileName> playbook.yaml
ansible-playbook -i ../inventory.ini playbook.yaml
```
I had the inventory.ini file in the parent directory of the current location.

Each playbook has 3 things, like 
- host
- remote_user -> like ubuntu user, root user 
- tasks -> to execute which tasks need to be done in the server

Modules are the one, which will execute the task, There are different types of modules, like shell, 

In the state, present means - install and absent means uninstall


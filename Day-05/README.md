Using Galaxy, we are downloading the role from ansible-galaxy and using in our play.

Command to install the role from ansible- galaxy
```
ansible-galaxy install <NameOfTheGalaxy
```

Then, write a playbook, and include the role that we have installed.

I have downloaded the docker role 
```
ansible-galaxy role install bsmeding.docker
```

Then create a playbook that has this role. 

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

When we want to publish, our role to the ansible-galaxy, we need to push to github and import to ansible-galaxy.
the token is generated in the collections section in ansible-galaxy

Command to import to the ansible-galaxy
```
ansible-galaxy import <GitHub-UserName> <Name of the Directory> --token <token>
ansible-galaxy import kalyankumar13 role-ansible --token 
```













-------------------------------------------------

The software will be installed in root user and group.  The purpuse of creating docker user and group is 
**Group**:
By adding other user to the docker group, we grant that user permissions to manage Docker containers, images, and other Docker-related resources. Users added to this group can manage Docker resources without needing to use sudo.
**User:**
User Can be used to run Docker services or tasks under a specific user account, further enhancing security and isolating processes.



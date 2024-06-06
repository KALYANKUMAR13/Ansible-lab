Roles:
To increase the readability and modularity , roles are used.
Each part of the play will be in particular folder and linked to particular play
The following command will manage the roles 
```
ansible-galaxy role init <nameOf the Role>
```

files are generated for that play in a structured manner.

Roles can be shared. Ansible Galaxy is kind of registry(dockerhub).

var - varibles folder, we can define the variables
tasks - things that we need to install
meta - version, data of the role ,author
handlers - Ansible task, when particular play aksed. In a play, we should be notified, so that particular task will run
files - Files that will be used in the play. Copy a particular file to all servers
template - similar to files, dynamic files
defaults - Variables - (default values)

If the files are alrady there, Ansible will not create.

Idempotency is a property of certain operations or API requests, which guarantees that performing the operation multiple times will yield the same result as if it was executed only once.

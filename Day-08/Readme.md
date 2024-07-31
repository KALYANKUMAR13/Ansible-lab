**Execuion of tasks:**

BY Default,
Ansible executes the tasks in order. If 1st task is completed successfully, then it goes to the 2nd task. If 1st task fails, it won't go further.

The below image says, to install docker in 10 hosts before that Check openssh and openssl  are installed in the latest version.
If it is not installed, ignore it and install the openssh ans openssl. Then go for  next tasks. 

By default, if a task is failed, it won't go to the next task.

<img width="926" alt="image" src="https://github.com/user-attachments/assets/0767096a-e106-4f11-b260-bad8d74dd0c4">

The image below is the code for the above scenario

<img width="476" alt="image" src="https://github.com/user-attachments/assets/04673f3e-e550-4ad2-abf4-b90f0eaaa65f">


If one task failed in the node, that host is ignored by ansible for further tasks, unless we mentioned the ignores error

<img width="521" alt="image" src="https://github.com/user-attachments/assets/2710a074-068f-4136-9dc4-6b3f8d0b94d1">



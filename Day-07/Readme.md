Ansible is **Idempotency**

 is a property of certain operations or API requests, which guarantees that performing the operation multiple times will yield the same result as if it was executed only once.

 When user tries to create 2 same configuration EC2 machine, Ansible will create only 1 as it is idempotant.

<img width="440" alt="image" src="https://github.com/user-attachments/assets/640bfa30-3c14-4256-8ba1-160458fb25c8">


The below code shutdown only the ubuntu (debian family)

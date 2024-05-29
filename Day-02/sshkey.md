For Vm in GCP, we need to generate ssh keys and attach to the vm

Step 1: Generate SSH Key Pair
Open terminal in wsl 
```
ssh-keygen -t rsa -b 2048 -C "your-email@example.com"
```

Follow the prompts:

Specify a file location: You can press Enter to accept the default file location (~/.ssh/id_rsa) or specify a different path.
Enter a passphrase: For added security, you can enter a passphrase. You can also press Enter to leave it empty.


Note the key files: The command generates two files:

~/.ssh/id_rsa (your private key)
~/.ssh/id_rsa.pub (your public key)

these file will be in 
```
cd /home/<Username>/.ssh
```
Copy the content of the public key and paste it to particular VM

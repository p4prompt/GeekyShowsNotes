### How to access server via ssh and setup ssh key for passwordless authentication
Without setting up SSH Key It will ask Password each time we try to get access

- To Get Access via SSH


Example:- ssh -p 21350 root@216.32.44.12
```

#### Note:- Run Below Commands on Your Local Machine, Not on Your VPS or Remote Server
- Generate SSH Key

ssh-keygen -t rsa -b 4096



2. Copy Public Key from descnition folder to vps


scp -P 22 id_rsa.pub u27653@216.32.44.12:/root/.ssh/authorized_keys

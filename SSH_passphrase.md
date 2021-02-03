### 1st, generate a pub key to .ssh
```
$ ssh-keygen -t rsa -b 2048
Generating public/private rsa key pair.
Enter file in which to save the key (/home/username/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/username/.ssh/id_rsa.
Your public key has been saved in /home/username/.ssh/id_rsa.pub.
```

### Copy your keys to the target server:
```
$ ssh-copy-id id@server
id@server's password: 
```

### Now try logging into the machine, with ssh 'id@server', and check in:
```
$ ssh id@server
```
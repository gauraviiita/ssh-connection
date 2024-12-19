# ssh-connection

**Connect to a Remote Server via SSH from Ubuntu**

Step 1: Install SSH on client (your local machine)
```
sudo apt update
sudo apt install openssh-client
```

Step 2: Install SSH on Server system
```
sudo apt update
sudo apt install openssh-server
```
Step 3: Verify the SSH server status on the remote machine:

```
sudo systemctl status ssh

systemctl status ssh
```
Ensure it says "active (running)." If not, start it with:
```
sudo systemctl start ssh
```

Step 4: Obtain the Server's IP Address
```
ip addr
```

Step 5: Connect to the Server

From the client machine, use the ssh command:
```
ssh username@server_ip
ssh gyadav@127.0.0.1
```
Enter the server login password 

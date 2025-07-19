## ssh-connection

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

```
Enter the server login password. 



### Connect to VPN:

Bielefeld VPN support page - [Support of the Faculty of Technology](https://www.google.com/search?q=techfak+vpn&oq=techfak+vpn&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIKCAEQABiABBiiBDIKCAIQABiABBiiBDIHCAMQABjvBTIHCAQQABjvBdIBCDUzNDlqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8#:~:text=VPN%20%2D%20Support%20of%20the%20Faculty%20of%20Technology)

download this [file](https://www.techfak.net/assets/files/openvpn-techfak-tcp.ovpn)

Command to connect with mosh

```
sudo apt install mosh
mosh gyadav@ebberg.techfak.uni-bielefeld.de
ssh gyadav@129.70.143.210
```

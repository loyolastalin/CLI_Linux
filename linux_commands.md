# reference 
[Youtube Video](https://www.youtube.com/watch?v=hQWRp-FdTpc)

# linux commands
[Userful commands](https://www.hostinger.in/tutorials/linux-commands)

# Find and Filter
- Find the version from the dotnet using grep and awk
```bash
 dotnet --info | grep -w "Version" | awk ' NR==1 {print $2}'
 ```
- Find the Free ram size in MB
```bash
 free -mt | awk  ' /Total/ {print $4}'
 ```
- Find the element with the space/tab delimter and get the element
 ```bash
 awk -F '[ ]' ' NR==2 {print $3}' test.txt
```

# SSH

## Password Authentication
- Manually give the password
```bash
ssh username@ipaddress
```
- Automate using sshpass
```bash
sshpass -p "passowrd" 
```
## Passwordless

- Generate SSH key 
```bash
ssh-keygen -t rsa -C "aa@aa.com"
```
- copy the public key to the server
```bash
ssh-copy-id username@ipaddress
```
- Connect to server
```bash
ssh username@ipaddress
```
# Userful comments
history
ls

## installing the package
sudo apt install apache2 -y

## secure Shell 

ssh-keygen

ls .ssh

cat .ssh/id_rsa.pub

cat ~/.ssh/id_rsa.pub | ssh demo@198.51.100.0 "mkdir -p ~/.ssh && chmod 700 ~/.ssh && cat >>  ~/.ssh/authorized_keys 

https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2





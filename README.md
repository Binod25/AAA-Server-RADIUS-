# AAA-Server-RADIUS-3.0
### Update Your Server:
```
sudo apt update
sudo apt upgrade -y
```
### Install FreeRADIUS:

```
sudo apt install freeradius freeradius-utils
```
### Configure FreeRADIUS:
 Edit the " clients.conf " file to add your client devices (like network access servers):
 ```
sudo nano /etc/freeradius/3.0/clients.conf
```
Add your client configuration. For example:
```
client localhost {
  ipaddr = 127.0.0.1
  secret = testing123
}
```
NOTE:- testing123 <Clint-Name> 

Edit the "users" file to define user accounts:


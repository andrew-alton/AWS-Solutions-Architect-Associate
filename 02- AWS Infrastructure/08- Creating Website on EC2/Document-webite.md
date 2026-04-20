```sh

sudo su -
yum -y install nginx
clear
 
systemctl status nginx
systemctl start nginx
systemctl status nginx
 
netstat -ntlp
 
 
cd /usr/share/nginx/html
cat index.html
echo "This is my first Website" > index.html
cat index.html

```

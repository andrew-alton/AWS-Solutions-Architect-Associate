```sh
### for Redhad distribution such as amazon linux, Redhat###

#!/bin/bash

# Update system
yum update -y

# Install nginx
amazon-linux-extras install nginx1 -y || yum install nginx -y

# Start and enable nginx
systemctl start nginx
systemctl enable nginx

# Get instance private IP
IP=$(hostname -I | awk '{print $1}')

# Create custom index.html
cat <<EOF > /usr/share/nginx/html/index.html
<!DOCTYPE html>
<html>
<head>
    <title>Server1</title>
    <style>
        body {
            background-color: blue;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        h1 {
            color: black;
            font-size: 3em;
            margin-bottom: 10px;
        }
        p {
            color: black;
            font-size: 1.2em;
        }
    </style>
</head>
<body>
    <h1>This is Server1</h1>
    <p>IP Address: $IP</p>
</body>
</html>
EOF

# Restart nginx
systemctl restart nginx

```

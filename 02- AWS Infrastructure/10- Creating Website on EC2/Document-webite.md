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
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        h1 {
            color: black;
            font-size: 3em;
        }
    </style>
</head>
<body>
    <h1>This is Server1</h1>
</body>
</html>
EOF

# Restart nginx to apply changes
systemctl restart nginx

```

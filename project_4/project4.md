# **PROJECT 4**
## MEAN STACK DEPLOYMENT TO UBUNTU IN AWS
### Install NodeJS
`sudo apt update`

`sudo apt upgrade -y`

`sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates`

`curl -sL https://deb.nodesource.com/setup_18.x | sudo -E bash -`

`sudo apt install -y nodejs`

### Install MongoDB
`sudo apt-get install gnupg`

`curl -fsSL https://pgp.mongodb.com/server-6.0.asc | sudo gpg -o /usr/share/keyrings/mongodb-server-6.0.gpg --dearmor`

`echo "deb [ arch=amd64,arm64 signed-by=/usr/share/keyrings/mongodb-server-6.0.gpg ] https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list`

`sudo apt-get update`

`sudo apt-get install -y mongodb-org`

![instal mongoDB](./images/install%20Mongod.png)

`sudo systemctl start mongod`

`sudo systemctl enable mongod`

`sudo systemctl status mongod`

![Mongod Status](./images/Verify%20Mongod.png)

`sudo npm install body-parser`

`mkdir Books && cd Books`

`npm init`

`vi server.js`
### Install Express And Setup Routes
`sudo npm install express mongoose`

`mkdir apps && cd apps`

`vi routes.js`

`mkdir models && cd models`

`vi book.js`

`cd ../..`

`mkdir public && cd public`

`vi script.js`

`vi index.html`

`cd ..`

`node server.js`

![Node Server](./images/server%20running%20node.png)

`curl -s http://localhost:3300`

![web app output](./images/web%20app%20output.png)
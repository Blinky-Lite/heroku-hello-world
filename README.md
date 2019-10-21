# heroku-hello-world

Download git repository to zip file
**wget https://github.com/dmcginnis427/heroku-hello-world/archive/master.zip**

Un-zip zip file
**unzip master.zip**

Rename unzipped directory to name of your choice
**mv heroku-hello-world-master my-heroku-hello-world**

Remove zip file
**rm master.zip**

Navigate to new directory
**cd my-heroku-hello-world**

Create and add variable to .env file
**echo "NODEREDCONFIGSECRET=a-secret-key" >> .env**

Install node modules
**npm install**

Run the Node-RED flow
**./run-blinky-lite.sh $(pwd)**


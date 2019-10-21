# heroku-hello-world

Download git repository to zip file<br>
**wget https://github.com/dmcginnis427/heroku-hello-world/archive/master.zip**

Un-zip zip file<br>
**unzip master.zip**

Rename unzipped directory to name of your choice<br>
**mv heroku-hello-world-master my-heroku-hello-world**

Remove zip file<br>
**rm master.zip**

Navigate to new directory<br>
**cd my-heroku-hello-world**

Create and add variable to .env file<br>
**echo "NODEREDCONFIGSECRET=a-secret-key" >> .env**

Install node modules<br>
**npm install**

Run the Node-RED flow<br>
**./run-blinky-lite.sh $(pwd)**


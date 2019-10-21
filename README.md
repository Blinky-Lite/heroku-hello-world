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

Create a new bcrypt password for editing the node-red flow<br>
**node -e "console.log(require('bcryptjs').hashSync(process.argv[1], 8));" *your-password-here***

and place this password in the settings.js file<br>
**nano settings.js**

in the adminAuth field<br>

Run the Node-RED flow<br>
**./run-blinky-lite.sh $(pwd)**

View flow at:<br>
**http://localhost:1880/admin**

The username is admin and the password is the one created above<br>


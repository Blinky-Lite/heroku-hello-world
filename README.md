# heroku-hello-world

1) Download git repository to zip file<br>
**wget https://github.com/dmcginnis427/heroku-hello-world/archive/master.zip**

2) Un-zip zip file<br>
**unzip master.zip**

3) Rename unzipped directory to name of your choice<br>
**mv heroku-hello-world-master my-heroku-hello-world**

4) Remove zip file<br>
**rm master.zip**

5) Navigate to new directory<br>
**cd my-heroku-hello-world**

6) Create and add variable to .env file<br>
**echo "NODEREDCONFIGSECRET=a-secret-key" >> .env**

7) Install node modules<br>
**npm install**

8) Create a new bcrypt password for editing the node-red flow<br>
**node -e "console.log(require('bcryptjs').hashSync(process.argv[1], 8));" *your-password-here***

9) and place this password in the settings.js file<br>
**nano settings.js**

in the adminAuth field<br>

10) Run the Node-RED flow<br>
**./run-blinky-lite.sh $(pwd)**

11) View flow at:<br>
**http://localhost:1880/admin**

The username is admin and the password is the one created above<br>

12) The html view is at:<br>
**http://localhost:1880/html**

13) The dashboard view is at:<br>
**http://localhost:1880/dashboard**

14) Exit the node-red flow:
**Control-C**

15) Log into heroku:
**heroku login**

16) Create a git repository:
**git init**

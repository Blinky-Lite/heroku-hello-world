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

14) Exit the node-red flow:<br>
**Control-C**

15) Log into heroku:<br>
**heroku login**

16) Go to a browser and log into your heroku dashboard:<br>
**https://dashboard.heroku.com**

17) Click ***New>>Create new app*** and Choose app name and region and click ***Create app***

18) Go back to your terminal window and create a git repository:<br>
**git init**

19) Add your heroku repository<br>
**heroku git:remote -a *your-app-name***

20) Add files to git repository<br>
**git add .**

21) Commit the files to the git repository<br>
**git commit -m "*your comments*"**

22) Push the files to heroku<br>
**git push heroku master**

23) Add the configuration variable in the .env file to the heroku site at:<br>
**https://dashboard.heroku.com/apps/***your-app-name***/settings**

click on the ***Reveal Config Vars** and add a KEY of **NODEREDCONFIGSECRET** with a value of **a-secret-key**

24) View flow at:<br>
**https://*your-app-name*.herokuapp.com/admin**

The username is admin and the password is the one created in Step 8 and 9<br>

25) The html view is at:<br>
**https://*your-app-name*.herokuapp.com/html**

26) The dashboard view is at:<br>
**https://*your-app-name*.herokuapp.com/dashboard**





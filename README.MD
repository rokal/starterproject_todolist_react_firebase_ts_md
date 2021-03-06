What does this project do? 
==========================
For more information on this project, please read this tutorial - http://developerlife.com/2016/10/02/getting-started-with-react-and-firebase/

Quick directions on getting this setup on my machine
====================================================
If you have a Mac and don't have `node` installed, then get `brew` and install `node` 
* ```/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```
* ```brew install node```

Initial Setup
-------------
* Go to the folder when you downloaded this project from github and run the following:
* `npm install babel webpack webpack-dev-server typescript typings -g`
* `typings install dt~node --global --save`
* `npm install`
* [more info on Node + Typescript](https://basarat.gitbooks.io/typescript/content/docs/quick/nodejs.html)

Firebase Setup in the [Firebase Console web app](https://console.firebase.google.com)
-------------------------------------------------------------------------------------
* Create a new project
* Set Database -> Rules to read/write by public using ```{
     "rules": {
       ".read": true,
       ".write": true
     }
   }```
* Set the Auth -> SignIn Methods to enable `Google` and `Anonymous`
* Put the config object generated by Firebase in `constants.js`
* When you deploy this to heroku, make sure to add your heroku app URL as an authorized domain in the Firebase console

Running it 
==========
For Dev
* `npm run dev`

For Prod
* `npm run postinstall`
* `npm run start`

Optional
========
* Install the React DevTools for Chrome [here](https://goo.gl/1XNSjY) 
* Install the Redux DevTools for Chrome [here](https://goo.gl/HTKf5g) 

See it in action
================
To see this app in action, here it is on heroku:
* https://todolist-redux-r3bl-alliance.herokuapp.com/

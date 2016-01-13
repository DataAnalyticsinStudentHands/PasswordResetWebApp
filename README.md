Password Reset Web App
===========

PasswordResetWebApp is a password reset service front end for most DASH applications. It handles requesting a passwords, receiving token from e-mail, and resetting the password.

This project is designed to connect to dynamic backends by using a webservice variable in the URL (via UI-Router) to determine which Java backend to connect to. The backend sends email with tokens that this application verifies is valid to perform activation, or password reset on a specific URL.

An working example of the PasswordResetWebApp can be found at [http://housuggest.org/PasswordReset/#/requestReset/FormBuilder](http://housuggest.org/PasswordReset/#/requestReset/FormBuilder) as it connects to the backend located on `/FormBuilder` and port `8443`.

### Development Prerequisites
- bower `npm install -g bower`
- gulp `npm install -g gulp`
- npm packages `npm install`

### Getting Started
1. Run `npm install`. This uses `package.js` to install local dependencies.
2. Run `gulp setup`. This runs common setup tasks, especially `bower install` using bower.json.
2. Run `ionic serve`. This uses `ionic.xml` and will serve as local node server. Live updates when you make changes to the code.

### Gulpfile
This repository is configured to deploy to Housuggest `gulp deploy-prod` and HnetDev `gulp deploy-dev` remote sites. Additional documentation [here](https://github.com/DataAnalyticsinStudentHands/DASH-Documentation/blob/master/Code%20Development/Frontend/App-Deployment-to-web-server.md).

Password Reset Web App
===========

PasswordResetWebApp is a password reset service front end for most DASH applications. It handles requesting a passwords, receiving token from e-mail, and resetting the password.

This project is designed to connect to dynamic backends by using a webservice variable in the URL (via UI-Router) to determine which Java backend to connect to. The backend sends email with tokens that this application verifies is valid to perform activation, or password reset on a specific URL.

### Getting Started
1. Run `npm install`. This uses `package.js` and install local dependencies.

1. Run `gulp setup`. This uses `Gulpfile.js` and sets up local repository.

2. Run `ionic serve`. This uses `ionic.xml` and will serve as local node server. Live updates when you make changes to the code.

# Node.js and Spotify API Playground

Followed along with this walkthrough: https://developer.spotify.com/documentation/web-api/quick-start/ 


## Goals

- [X] Create a simple application using Node.js and JavaScript
- [X] Register an application with Spotify
- [X] Authenticate a user and get authorisation to access user data
- [X] Retrieve the data from a Web API endpoint


## Notes

Actions:
* created a test server file (server.js)
* cloned "OAuth examples" files into this folder (from https://github.com/spotify/web-api-auth-examples)
* installed dependencies by running "npm install" in the terminal
* mitigated one high severity vulnerability (https://nodesecurity.io/advisories/1464) by uninstalling and reinstalling express and request via NPM
* logged into Spotify developer site
* created a Spotify app in the developer dashboard and then configured it's redirect URI to "http://localhost:8888/callback"
* configured app to use my Spotify client ID and secret (in authorization_code's app.js file)
* ran the default app using "cd authorization_code" and then "node app"
* tested the app by following Spotify sign in steps
* the final result is a page displaying the signed in Spotify account details
* see original repo details below:


# Spotify Accounts Authentication Examples

This project contains basic demos showing the different OAuth 2.0 flows for [authenticating against the Spotify Web API](https://developer.spotify.com/web-api/authorization-guide/).

These examples cover:

* Authorization Code flow
* Client Credentials flow
* Implicit Grant flow

## Installation

These examples run on Node.js. On [its website](http://www.nodejs.org/download/) you can find instructions on how to install it. You can also follow [this gist](https://gist.github.com/isaacs/579814) for a quick and easy way to install Node.js and npm.

Once installed, clone the repository and install its dependencies running:

    $ npm install

### Using your own credentials
You will need to register your app and get your own credentials from the Spotify for Developers Dashboard.

To do so, go to [your Spotify for Developers Dashboard](https://beta.developer.spotify.com/dashboard) and create your application. For the examples, we registered these Redirect URIs:

* http://localhost:8888 (needed for the implicit grant flow)
* http://localhost:8888/callback

Once you have created your app, replace the `client_id`, `redirect_uri` and `client_secret` in the examples with the ones you get from My Applications.

## Running the examples
In order to run the different examples, open the folder with the name of the flow you want to try out, and run its `app.js` file. For instance, to run the Authorization Code example do:

    $ cd authorization_code
    $ node app.js

Then, open `http://localhost:8888` in a browser.

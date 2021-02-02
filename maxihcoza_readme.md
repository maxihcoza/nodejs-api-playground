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
# PWA-Text-Editor

## Description

The goal of this assignment is to  build a single-page text editor that runs in the browser and can be installed locally by the user. It also features a number of data persistence techniques in case one of the allotted options aren't supported. It also features IndexDB which is useful for storing and retrieving data.

```
GIVEN a text editor web application
WHEN I open my application in my editor
THEN I should see a client server folder structure
WHEN I run `npm run start` from the root directory
THEN I find that my application should start up the backend and serve the client
WHEN I run the text editor application from my terminal
THEN I find that my JavaScript files have been bundled using webpack
WHEN I run my webpack plugins
THEN I find that I have a generated HTML file, service worker, and a manifest file
WHEN I use next-gen JavaScript in my application
THEN I find that the text editor still functions in the browser without errors
WHEN I open the text editor
THEN I find that IndexedDB has immediately created a database storage
WHEN I enter content and subsequently click off of the DOM window
THEN I find that the content in the text editor has been saved with IndexedDB
WHEN I reopen the text editor after closing it
THEN I find that the content in the text editor has been retrieved from our IndexedDB
WHEN I click on the Install button
THEN I download my web application as an icon on my desktop
WHEN I load my web application
THEN I should have a registered service worker using workbox
WHEN I register a service worker
THEN I should have my static assets pre cached upon loading along with subsequent pages and static assets
WHEN I deploy to Heroku
THEN I should have proper build scripts for a webpack application

```

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contributions](#contributions)
- [License](#license)
- [Tests](#tests)
- [Questions](#questions)

## Installation

In order to install the app, first run "npm i" in both the server and client folders to create the "node_modules" and "package-lock.json" and then install webpack using "npm i webpack" in the terminal. Also make sure that the package.json in the root folder includes these dependencies:

```
"scripts": {
    "start:dev": "concurrently \"cd server && npm run server\" \"cd client && npm run dev\"",
    "start": "npm run build && cd server && node server.js",
    "server": "cd server nodemon server.js --ignore client",
    "build": "cd client && npm run build",
    "install": "cd server && npm i && cd ../client && npm i",
    "client": "cd client && npm start"
  },

```
The app should run from the root in the package.json using "npm start".

## Usage

The application should be used as a text editor to store your thoughts or whatever is on your mind. It can also be installed into your local computer. To view the app.

## Contributions

N/A

## License

N/A

## Tests

N/A

## Questions

- Github: https://github.com/jmaduafo

## Screenshots

[jate1.webm](https://github.com/jmaduafo/PWA-Text-Editor/assets/87540591/ee319d71-e46d-4b45-8628-e9326c7329b2)

[jate2.webm](https://github.com/jmaduafo/PWA-Text-Editor/assets/87540591/9e07e934-445a-46d9-800f-d46eb8264398)

Angular4-WithAPI-github.io

This repository holds the source code of the angular.io Angular4 using IMDB database.This is basically involved in getting data from IMDB provided movies API and displaying it on the browser.

It's been extended with testing support so you can start to use these test cases and extend them if needed.

Prerequisites

Node.js and npm are essential to Angular development.

Get it now if it's not already installed on your machine.

Verify that you are running at least node v4.x.x and npm 3.x.x by running node -v and npm -v in a terminal/console window. Older versions produce errors.

Clone this repo into new project folder (e.g., new-proj).

git clone https://github.com/SriVaishnaviAkula/Angular4-WithAPI.git new-proj cd new-proj

You could start writing code now and throw it all away when you're done. If you'd rather preserve your work under source control, consider taking the following steps.

Steps To Run angular

npm install npm start

The npm start command first compiles the application, then simultaneously re-compiles and runs the lite-server. Both the compiler and the server watch for file changes.

Shut it down manually with Ctrl-C.

You're ready to write your application.

Testing The Application

npm test - compiles, runs and watches the karma unit tests npm run e2e - run protractor e2e tests, written in JavaScript (*e2e-spec.js) Testing

Unit Tests

TypeScript unit-tests are usually in the app folder. Their filenames must end in .spec.

Look for the example app/app.component.spec.ts. Add more .spec.ts files as you wish; these are configured using karma.

Run it with npm test

That command first compiles the application, then simultaneously re-compiles and runs the karma test-runner. Both the compiler and the karma watch for (different) file changes.

Shut it down manually with Ctrl-C.

Test-runner output appears in the terminal window. We can update our app and our tests in real-time, keeping a weather eye on the console for broken tests. Karma is occasionally confused and it is often necessary to shut down its browser or even shut the command down (Ctrl-C) and restart it.

End-to-end (E2E) Tests

E2E tests are in the e2e directory, side by side with the app folder. Their filenames must end in .e2e-spec.ts.

Look for the example e2e/app.e2e-spec.ts. Add more .e2e-spec.js files as you wish. these are configured using protractor to find them.

Thereafter, run them with npm run e2e.

That command first compiles, then simultaneously starts the Http-Server at localhost:8080 and launches protractor.

The pass/fail test results appear at the bottom of the terminal window. A custom reporter (see protractor.config.js) generates a ./_test-output/protractor-results.txt file which is easier to read; this file is excluded from source control.

Shut it down manually with Ctrl-C.

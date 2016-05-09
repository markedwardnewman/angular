# AngularJS Phone Catalog Application
###[Live Demo](https://morning-lowlands-91358.herokuapp.com)

- This app is a catalog that displays a list of Android devices, lets you filter the list to see only devices that interest you, and then view the details for any device.  Built from the ground-up, it is a slightly modified version of an advanced Angular tutorial found [here](https://angularjs.org/).
- Once I had it working I deployed it to Heroku following the steps shown [here](http://linqed.eu/2014/10/07/deploying-angular-seed-to-heroku/).

## Workings of the application
- The application filesystem layout structure is based on the [angular-seed] project.
- There is no dynamic backend (no application server) for this application. Instead the application server is faked by fetching static json files.

### Installing dependencies
- The application relies upon various node.js tools, such as Bower, Karma and Protractor.  You can install these by running:
```
$ npm install
```
- This will also run bower, which will download the required angular files.

### Running the app during development
- Run `npm start`
- navigate your browser to `http://localhost:8000/app/index.html` to see the app running in your browser.

### Running unit tests
- Start Karma with `npm test`
  - A browser will start and connect to the Karma server. Chrome is the default browser, others can be captured by loading the same url as the one in Chrome or by changing the `test/karma.conf.js` file.
- Karma will sit and watch your application and test JavaScript files. To run or re-run tests just change any of your these files.

### End to end testing
- Requires a webserver that serves the application.
- Serve the application: run `npm start`.
- In a separate console run the end2end tests: `npm run protractor`. Protractor will execute the end2end test scripts against the web application itself.
  - The configuration is set up to run the tests on Chrome directly. If you want to run against other browsers then you must install the webDriver, `npm run update-webdriver`, and modify the configuration at `test/protractor-conf.js`.

## Application Directory Layout
    app/                --> all of the files to be used in production
      css/              --> css files
        app.css         --> default stylesheet
      img/              --> image files
      index.html        --> app layout file (the main html template file of the app)
      js/               --> javascript files
        app.js          --> the main application module
        controllers.js  --> application controllers
        directives.js   --> application directives
        filters.js      --> custom angular filters
        services.js     --> custom angular services
        animations.js   --> hooks for running JQuery animations with ngAnimate
      partials/         --> angular view partials (partial html templates) used by ngRoute
        partial1.html
        partial2.html
      bower_components  --> 3rd party js libraries, including angular and jquery
    test/               --> test source files and libraries
      karma.conf.js        --> config file for running unit tests with Karma
      protractor-conf.js   --> config file for running e2e tests with Protractor
      e2e/
        scenarios.js       --> end-to-end specs
      unit/             --> unit level specs/tests
        controllersSpec.js --> specs for controllers
        directivesSpec.js  --> specs for directives
        filtersSpec.js     --> specs for filters
        servicesSpec.js    --> specs for services

## Contact
###Mark Newman - Front End Web Developer

**Portfolio:** [markedwardnewman.com](http://markedwardnewman.com "markedwardnewman.com")

**Location:** Austin, TX, United States

**Email:** markedwardnewman@gmail.com

**Download:** [résumé](http://www.markedwardnewman.com/assets/other/misc/MarkNewmanResume.docx)

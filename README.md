### Issues and findings

Using https://github.com/Workiva/karma-jspm, which works for system but has a slight issue loading files with .ts extension. 

Opened a PR for this : https://github.com/Workiva/karma-jspm/pull/79

A second issue I've had was that I had to wget system-polyfills.src.js into jspm_packages, karma-jspm expected it there, but it was not there. 

### Steps to use this project

```npm install```

```jspm install```

#### Run the tests

```karma start```

#### Run the web server

```npm start```

#### Do a JSPM build

https://github.com/jspm/jspm-cli/blob/master/docs/production-workflows.md

TLDR : 

```jspm bundle-sfx src/app.ts! dist/build.js```
( warning currently this is not working, will investigate asap )




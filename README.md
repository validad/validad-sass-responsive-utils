#RESPONSIVE UTILS FOR SASS (by Validad AG)

***

##1. QUICKSTART
Install Node.js and then:

```sh
$ git clone git://github.com/validad/validad-sass-responsive-utils
$ cd validad-sass-responsive-utils
$ npm install
$ npm bower
```

##2. PURPOSE
The purpose of this project it's developing sass unit tests focused on responsive web desgin.

##3. OVERALL DIRECTORY STRUCTURE
At a high level, the structure looks roughly like this:
```
.
├── bower_components/
│   └── bootcamp
├── bower.json
├── config.rb       
├── config.specs.scss
├── node_modules/     
│   ├── bootcam/
│   ├── grunt/
│   └── grunt-contrib-sass/
├── package.json
├── src/
│   ├── _mixins/
│   └── main.scss
└── test/
```

What follows is a brief description of each entry:
- `bower_components` : third-party libraries. [Bower](http://bower.io) will install
  packages here. Anything added to this directory will need to be manually added
  to `config.specs.scss` to be picked up by the build system
- `bower.json` : this is our project configuration for Bower and it contains the
  list of Bower dependencies we need.
- `config.rb` : our Compass configuration for this project.
- `config.specs.scss` : our test configuration to run them.
- `node_modules` : third-party libraries. [Npm](https://www.npmjs.org/) will install
  packages here. Anything added to this directory will need to be manually added
  to `config.specs.scss` to be picked up by the build system
- `package.json` - metadata about the app, used by NPM and our build script. Our
  NPM dependencies are listed here.
- `src/` - sources to be tested.
- `test` - tests

##4. HOW TO WRITE A TEST WITH BOOTCAMP

source: http://thejameskyle.com/bootcamp/#!/wiki/Introduction

##5. HOW TO RUN A TEST
   To run Bootcamp and get the results of the test suite simply compile the config.specs.scss

```sh
$ sass config.specs.scss
```
About [sass] (http://sass-lang.com/install)

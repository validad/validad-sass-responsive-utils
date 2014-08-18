RESPONSIVE UTILS FOR SASS (by Validad AG)
------------------------------------------

1. PURPOSE
   The purpose of this project it's developing sass unit tests focused in responsive web desgin.

2. INSTALLATION DEPENDENCIES
   2.1 In our project we use Bootcamp to develop unit tests(http://thejameskyle.com/bootcamp/).
        Npm:   npm install --save-dev bootcamp
        Bower: bower install --save-dev bootcamp

   2.2 After installing Bootcamp  add it to your Sass :load_paths, instructions for Grunt and Compass:
        npm   './node_modules/bootcamp/dist'
        bower './bower_components/bootcamp/dist'

   2.3 Then setup your sass files for writing tests. Create config.specs.scss on root directory
        config.specs.scss:
        @import "src/foo";

        @import "bootcamp"; // or "[node_modules|bower_components]/bootcamp/dist/bootcamp" if you didn't set load_paths
        $bc-setting-verbose:  false;
        $bc-setting-warnings: false;

        @include runner-start;
        @import "test/foo.scss";
        @include runner-end;

  2.5 Compass
        config.rb
        syntax = :scss
        css_dir = './build'
        sass_dir = './src'
        output_style = :expanded

        add_import_path './node_modules/bootcamp/dist' # or './bower_components/bootcamp/dist'

  2.6 Project's structure we use
        .
        ├── bower_components            //using Bower
        │   └── bootcamp
        ├── bower.json
        ├── config.rb                   //Compass
        ├── config.specs.scss
        ├── node_modules                //Using Npm
        │   ├── bootcam
        │   ├── grunt
        │   └── grunt-contrib-sass
        ├── package.json
        ├── src                         //Source folder
        │   └── functions
        └── test                        //Testing folder
            └── functions

3. HOW TO WRITE A TEST WITH BOOTCAMP

   source: http://thejameskyle.com/bootcamp/#!/wiki/Introduction

4. HOW TO RUN A TEST
   To run Bootcamp and get the results of the test suite simply compile the config.specs.scss

        sass config.specs.scss


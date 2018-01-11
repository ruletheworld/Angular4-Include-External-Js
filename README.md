# Angular4-Include-External-Js
Angular 4 Include External Javascript /JQuery 

For including your custom javascript / jquery files in angular project follow below given steps.

Step 1 : create your custom js file labelled as 'sample.js' and place it in angularproject\src\assets\externaljs\sample.js

Step 2 : Open / Edit Angular Project search for .angular-cli.json (it will be located in root dir)

Step 3 : Search Tag   "scripts": [], and give your custom js path here 
Example : "scripts" : ["assets/externaljs/sample.js"] 
--tips 1 :  By default your current directory path will be angularproject/src/
--tips 2 : U can place multiple js files path here by using comma separator as "scripts" : ["assets/externaljs/sample.js","assets/externaljs/sample2.js","assets/externaljs/sample3.js"] 

step 4 : I am considering that you have already created components in your angular project.
Open / Edit your app.component.ts file and declare variable as 
declare var myjsfunction: any;
here myjsfunction will be you custom js / jq function which is defined in your custom js/jq file.

step 5 : Once you declare var myjsfunction : any
you can now place your javascript functions whereever it is required in you app.component.ts file.



credits : querynext.com


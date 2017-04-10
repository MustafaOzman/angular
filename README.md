# angular/cli
# Refe: https://cli.angular.io or https://github.com/angular/angular-cli
#check node version 
node -v
#usefull command for creating, building, deployment and testing(unti and end to end)
# install cli globally 
npm i @angular/cli -g   
#check cli version
ng -v
#check cli insalled and exist  , --depth=0 to view the name only
npm list -g @angular/cli  --depth=0
# create new project with the main files 
ng new my-project
# creat project without installing on the local pc, skip npm install
ng new my-project --skip-install
#cd to my-project then 
ng serve 
# open browser to localhost:4200 to view the running app
#to find decumentation about components via website
ng doc component
# view many command with differant features 
ng --help
#learn about ng serve command
ng serve --help

ng lint
# unit testing 
ng test
# end to end testing 
ng e2e
# deploy the application which will output the application in dist folder
ng build 
# 
ng serve --prod

#ngModule and Routing 
ng g module admin
#create project with routing and dry run with routing module and app module
ng new newproject --routing -d
#Example of routing from:
http://angular2-first-look.azurewebsites.net/
#generate new module and its routing 
ng g m admin --routing 
#generate component in admin module
ng g c admin/users


#Generate Guard auth
ng g guard auth

#Building and dyploying the app into dist folder as defined in angular-cli.json as outDir
ng build
#analyze the sourcemap to draw a dependancy map, Reveals exactly which modules and classes are in the bundle 
https://github.com/danvk/source-map-explorer
# tool installed to manage the build bundles to optomize code in size 
npm install source-map-explorer --save-dev
#run the tool in the browser to view the builded bundles contents with files size 
./node_modules/.bin/source-map-explorer dist/main.bundle.js     
#type of Builds
#  Environment Build to indicate which file to use between environment.prod.ts and environment.ts
#Target build to define how and if the files to be optimized
#sm:source map is optional which used to view the file size in the browser when the project is builded 
ng build --prod -sm
ng build --prod 
ng build --aot
ng build --help

#run the ng command automatically when loading the app without using cli
# use ng eject to generate webpack configration in the project 

#using angular material 
ng i @angular/material --save

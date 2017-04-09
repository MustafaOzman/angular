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



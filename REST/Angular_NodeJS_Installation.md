Platform: Ubuntu 20.04 (Windows 10 - Build 2004 - WSL2)

##Install and Test NodeJS

Reference : https://mdbootstrap.com/education/angular/installation-lesson-1/  

1. Install NodeJS: "sudo apt-get install -y nodejs"
2. Install NPM: "sudo apt-get install -y npm"
3. Test NodeJS: "node -v" -> v10.19.0
4. Test NPM: "npm -v" -> 6.14.4
5. Verify: "echo 'console.log("Hello");' > hello.js" , "node hello.js" -> Hello

##Install Angular CLI

Reference : https://angular.io/guide/setup-local  

1. Install Angualr CLI : "sudo npm install -g @angular/cli"
2. Create new app: "ng new frontend", ? Would you like to add Angular routing? (y/N) y, ? Which stylesheet format would you like to use? CSS
3. Change homepage : "echo Hello > frontend/src/app/app.component.html"
4. Test app: "cd frontend/" , "ng serve --open"

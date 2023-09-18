## make a file (addFive.js) with function definition and then 
## write module.exports=addFiveso  so that it can be used by other  files in this folder
********now check if node js and npm install or not*********
in terminal
## type node --version this gives v20.5.1 means installed
## type npm --version this gives 9.8.0
*********check if jest is installed*************
## type jest --version
this gives comand just not found meaning not installed so we have to install it here
so we install it using npm because npm is the way to install node modules into our web projects
********installation**********
## type and run npm init -y
to add a pakage.json file 
-y automatically answer yess to all the questions init command asked during nstallation
**now i have a pakage.json file** 
in other words i have a way to keep track of node modules that this project depends on 
## jest installation
since i want to use jest testing library so i need to install it locally means installing it for the project 
for this run 
**nmp install --save-dev jest**
after few minutes the pakage.json file will be updated by jest testing library
now in the pakage.json file we need to do some cahanges in the script section
**in the test entry write jest by removing other text**
now run the command
npm run test
this will run the jest command in this folder 
what will this command do?
it runs tests for the cose in my project
right now i have a single file addFive.js so it makes sense to creat a test file for this 
i'll name it addFive.test.js 
in this write
const addFive= require(`./addFive.js`);
test('returns the number plus 5', ()=>{
    expect(addFive(1)).toBe(6);
} )
**then run the command**
## npm run test
we will get pass message in terminal

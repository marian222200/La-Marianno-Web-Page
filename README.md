# La-Marianno-Web-Page

A prototype of La Marianno Web Page for pizza delivery. My first try at front-end (back in 2019).

## How to run the project

The client side of the project I ran using this [extension](https://github.com/ritwickdey/vscode-live-server-plus-plus "GitHub: Vscode Live Server++ (BETA)"). For the server side I used [Node.js](https://nodejs.org/en/about/ "About Node.js").
To start the server you need to have Node.js installed and run *node server.js* in comand line in the project folder.

## Main page

The main page consists of the login and register buttons, and a catalog for the avabile pizza. You have to be logged in in order to order and give a rating. The list of pizza is received from the hosted server. For more info, check the server part down below.


![image](https://user-images.githubusercontent.com/30511514/172068357-af4af46e-16f2-4626-a932-0578ad2696b8.png)

## Login form

If you press the Login button the login form is shown. You need to be registered in order to log in. If you try to enter a non existing email, an alert saying the user is not existent will be shown. If you try to log in into an existing user more than 5 times without entring the right password you will get a time-out that prevents you from trying again for a certain time.

![image](https://user-images.githubusercontent.com/30511514/172069118-1cbebef5-dda5-40c0-bd57-0e99a94ae760.png)

## Register form

If you press the Register button, the Register form is shown. In order to register you need to have first name, last name, a valid email, and a valid password. All the validation is made using [Regular Expresions](https://www.youtube.com/playlist?list=PL55RiY5tL51ryV3MhCbH8bLl7O_RZGUUE "Regular Expresions Tutorial YouTube Playlist").

![image](https://user-images.githubusercontent.com/30511514/172069961-b1c5ffaa-4c73-435b-8b33-570364026571.png)

## Adding pizza form

Once you have logged in successfully the page refreshes and you then have the button to open the adding pizza form.

![image](https://user-images.githubusercontent.com/30511514/172069577-b223e31d-dde3-4b23-ae14-b544789d0f3a.png)

## Info last login

Another button that is shown once you are logged in is the *Info logare* button that shows you the list of the previous logins (the current one is not includded). 

![image](https://user-images.githubusercontent.com/30511514/172069637-85f5fbbd-18da-4986-a496-56ac8da39405.png)

## Server Side

The app does not have a data-base. All the information is lost upon restarting the Node.js server. The server is responsible for returning the list of pizza upon request, login form, register form, pizza rating. The server also is responsible for returning error codes if the request get declined. The server used to sent emails back in 2019 using a gmail account, but google updated their terms and conditions since then and the app does not sent emails anymore :(.

## Http Requests

The Requests to the server were made using Fetch API. For more info visit this [tutorial](https://www.youtube.com/watch?v=23hrM4saaMk "Fetch API tutorial").

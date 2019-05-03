![Screenshot](https://microsites.nbg.gr/api.gateway/publicportal/sites/default/files/2018-11/black_logo.jpg) 
# Developer Studio User Guide
By introducing **NBG Developer Studio**, NBG's effort is to help developers continue their hard work on the cloud, without having to install dependencies on their host machines and also take advantage of the resources of this platform. That way, a developer can continue his work from everywhere in the world.
## Login
By visiting https://studio.developer.nbg.gr you are redirected to NBG's Login Page. To access NBG's **Developer Studio** you need to have an active account on NBG's Identity Server. If it is your first time, feel free to create one by clicking **Sign Up**
![Screenshot](https://files.nbg.gr/studio/login.PNG) 
## Menu Buttons
-- **Account Settings**<br />
![Screenshot](https://files.nbg.gr/studio/account-settings.PNG) <br />
*By clicking the account settings button, you can check your account information and customize your developer experience by changing the theme and/or editor settings*<br />
-- **Start a Project**<br />
![Screenshot](https://files.nbg.gr/studio/start-project.PNG) <br />
*By clicking Start a Project, you can start by creating a project from scratch or clone an existing project from github*<br />
-- **Switch Project**<br />
![Screenshot](https://files.nbg.gr/studio/switch-project.PNG)<br />
*If you have more than one projects on **Studio Developer** you can navigate to them by clicking the Switch Project button*<br />
-- **Open the Handbook**<br />
![Screenshot](https://files.nbg.gr/studio/handbook.PNG)<br />
*This one is pretty straight forward. It's a link to me! :) Check on me, every now and then, just to make sure I am ok*<br />
-- **Ask for some help**<br />
![Screenshot](https://files.nbg.gr/studio/help.PNG)<br />
*That is the place to find the necessary information if you feel like contacting us*

## Starting a Project
The first time that you login, you see the default homepage which indicates that you have completed successfully the login process. On this page, it is very clear that you haven't started any projects yet. 
![Screenshot](https://files.nbg.gr/studio/homepage.PNG)
By clicking the big Plus Sign (+) button you can start the flow of creating a new project. There are 2 options. Start a project from scratch or clone an existing repo.<br />
![Screenshot](https://files.nbg.gr/studio/start-project.PNG) ![Screenshot](https://files.nbg.gr/studio/start-project-2.PNG)
### From Scratch
By choosing ***From scratch***, NBG is giving you the option to start a project of one of the supported languages by ***studio.developer.nbg.gr***. Currently the supported languages are: 
* Python (version 3.6.4)
* Node.js (version 8.9.4)
* PHP (version 5.5.9)
* .NET Core (version 2.1.4)

![Screenshot](https://files.nbg.gr/studio/from-scratch.PNG)<br />
By default NBG provides a sandbox template with some rest calls to help you get started with the platform and NBG APIs.

### Clone a repo
If you have a github repo with your personal code, you can clone it and run it on ***https://studio.developer.nbg.gr***
That way, you can continue the development of your own code on **Developer Studio**. 
![Screenshot](https://files.nbg.gr/studio/clone-from-repo.PNG)
## Inside the Project 
The first page you see everytime you start a new project, is the README.md page which has some information about the specific project. NBG provides a sample application which is able to execute some simple rest calls to a specific NBG API. The goal is to get you started and help you experiment with the platform and the APIs at the same time.
Now that you are in a project, you can see many new features. Let's seperate them in sections:
-- **File Explorer Menu**
-- **File Editor**
-- **Logs and Terminal**
-- **Main Menu**
### File Explorer Menu
![Screenshot](https://files.nbg.gr/studio/file-explorer.PNG)<br />
In this section of the screen, you can see the files of your project and also manage them. On the menu of this section, You can create folders, files and even upload as many as you want from your local machine. In addition, there is a search bar to help you navigate through folders, if you know which file you want to open on the file browser.
### File Editor
![Screenshot](https://files.nbg.gr/studio/file-editor.PNG)<br />
This is the place where the files are being opened. It's also the place, where you write your code and save it. The editor is customizable and there are plenty themes that you can choose from so it matches your personal preferences.
### Logs and Terminal
![Screenshot](https://files.nbg.gr/studio/command-line.PNG)<br />
This is the most confusing (for some) section of your project screen. Depending on your project you may see different tabs. Each tab has its own purpose. On the **Console** tab you can see the logs of your project's activity, if it is developed in that way. On the **Server Logs** tab you can see the logs of the web server that is hosting your application. Last but not least, the **Terminal**, which is the most important one. From that tab you are able to execute commands in the shell like you would normally do on your local machine.
### Main Menu
This menu is enriched with buttons that give you better control over your project. There are 3 sections that are added in this menu.
1. Github Buttons<br />
![Screenshot](https://files.nbg.gr/studio/github-buttons.PNG)<br />
With these buttons you can commit / push / pull clone code from your repo. Before that though, you have to have linked your code with a repo if you haven't cloned an existing one. There is this helpful article [article](https://help.github.com/en/articles/adding-an-existing-project-to-github-using-the-command-line) on how to do that from the command line.
2. Toggle Buttons<br />
![Screenshot](https://files.nbg.gr/studio/toggle-buttons.PNG)<br />
With these buttons you can toggle the terminal / command palette / file explorer on and off as you please, in order to have more space for the file editor.
3. Server Buttons<br />
![Screenshot](https://files.nbg.gr/studio/server-buttons.PNG)<br />
These buttons are responsible for running your application on a webserver. The first button is to start/stop your application and the second one is for browsing the public url of your application.
![Screenshot](https://files.nbg.gr/studio/public-url.PNG)<br />
***CAUTION*** <br />
Every project that you want to run and be able to browse its public url needs to have a Procfile. More information about that [here](https://help.sourcelair.com/webserver/procfiles/)<br />
Every project runs on a container behind a reverse proxy .<br />
Default exposed containter ports per container type are

|                |PORT                          
|----------------|------------------------------
|Node|`3000`            
|Python|`8000`
|NET.Core|`5000`
|PHP|`8000` no procfile needed


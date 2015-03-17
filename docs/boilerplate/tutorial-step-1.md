#"Grunt" Work
Grunt is a build tool that will handle and automate all of the nitty-gritty for you. You use it by invoking predefined "tasks" via the command line. The following sections describe how and what it can do for you.

**Using the Grunt CLI (Command-line Interface)**  
Open the terminal and make sure you switch to your project directory using `cd` or similar. Once inside your project directory you'll simply type `grunt` followed by your desired command (detailed below).

<img src="../img/cmd-grunt.gif"/>

###Working Locally

In your terminal type `grunt` followed by the enter key. Grunt will start a live preview server and open the boilerplate preview inside your default browser.  

The live preview server allows you to change theme settings and preview them locally in your web browser as you work. This creates an easy way to tweak and see your changes happen in (almost) real time.  

> **Note:** Once you've started the server it will continue to run and watch for changes to the project files. When you want to stop the server press `ctrl+c` or simply close your terminal window.

###Creating A Theme

Instead of having multiple folders or directories for multiple themes you will use a **single folder** for **all** of your themes. This is possible since we are using Git to manage our changes and revisions.

In your terminal type `grunt new_theme` followed by the enter key. You will receive the following prompts:

* **Theme Group Id**  
The group id is a value generated in the system once a group has been created. If you intend on publishing your theme you'll need to have this value ready before continuing. For the purposes of this tutorial you can type `demo` followed by the enter key.

* **Theme Name**  
The theme name can be whatever you'd like, typically it will be the name of the group that the theme belongs to. Please use initial-caps and spaces.  

>> **Good Name:** "My Awesome Name"  
>> **Bad Name(s):** "mybad_name", "my bad name", "My bad name"  

* **Copy Existing Theme**  
This option allows you to select another theme as a starting point. For the purposes of the tutorial select `No` followed by the enter key.

<img src="../img/cmd-new_theme.gif"/>

###Additional Info - Copying Existing Themes
If you select `Yes` in the previous step, you'll be prompted to enter the desired theme's name. If you don't enter a value and press the enter key, you will see a listing of all available themes. If you type a value it will be used to search/filter the available themes.

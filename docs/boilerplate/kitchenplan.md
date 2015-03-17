#Why Do I Have to Install Stuff?
The boilerplate themes are generated via a specific set of tools that must be installed on your system. Once installed you'll be ready to start generating themes! Once you've completed either the Full or Basic installation below, please proceed to the [setup instructions](boilerplate/setup).

###Full Installation - Mac OSX (Recommended)
Following the instructions below will setup the automated installer [Kitchenplan](http://kitchenplan.github.io/kitchenplan/) and use our custom configuration to get your system up to speed in no time!

- **Sublime Text 3** - Preconfigured with extensions, etc
- **Sourcetree** - Version control for working with GitHub
- **NodeJS** - Server for live-reload and build tools
- **SASS** - CSS Preprocessor
- **Grunt** - Build tool for compiling and publishing themes
- **TotalTerminal** - Makes OSX's Terminal.app easier to access and use

***

**IMPORTANT: ** Before proceeding with the Kitchen plan install we'll need to add your OSX user name to the configuration files, please contact <casey.corcoran@lightspeedvt.com> first!

1. Open Applications/Utilities/Terminal.app

2. Update Ruby Gems:  
`sudo gem update --system`

3. Install Kitchenplan:  
`sudo gem install kitchenplan`

4. Run Kitchenplan setup:  
`kitchenplan setup`

5. At the prompt:  
`Do you have a config repository? [y,n]` type `y` and press enter

6. At the prompt:  
`Please enter the clone URL of your git config repository:` paste this url: `https://github.com/lightspeedvt/boilerplate-config.git` and press enter

7. Once setup has completed type:  
`kitchenplan provision` and press enter  
All of the various tools will be installed and the process should complete after a while. Note that due to a bug, step 7 must be done manually and is not automated via Kitchenplan.

7. Install SASS  
`sudo gem install sass`

***

###Basic Installation - Windows, Linux, Etc
The minimum tools you'll need on any system to compile and publish themes are listed below:

1. **SASS -** [Installation Instructions](http://sass-lang.com/install)
2. **NodeJS -** [Installation Instructions](http://nodejs.org/)
3. **Grunt CLI -** [Installation Instructions](http://gruntjs.com/getting-started)
4. **Bower -** [Installation Instructions](http://bower.io/#install-bower)

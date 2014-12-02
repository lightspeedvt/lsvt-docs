#Getting Started - Mac OSX

##Required Tools
The boilerplate themes are generated via a specific set of tools that must be installed on your system. Once installed you'll be ready to start generating themes!

##Automated Installation
The various tools and utilities can be installed automatically using [Kitchenplan](http://kitchenplan.github.io/kitchenplan/)

1. Update Ruby Gems

    >`sudo gem update --system`

2. Install Kitchenplan

    `gem install kitchenplan`

3. Run Kitchenplan setup

    `kitchenplan setup`

4. Set config repository
    Kitchenplan will prompt you with the following, type `y` and press enter:

    `Do you have a config repository? [y,n]`

##Manual Installation

###Sass

1. **Install the Ruby "Gem"**
    Open Applications/Utilities/Terminal.app and paste the following code, then hit enter.

    `gem install sass`

2. If you receive an error, add `sudo` and try again, you will be prompted for your password.

    `sudo gem install sass`

[Full Instructions Here](http://sass-lang.com/install)

###Grunt

1. **Download and run NodeJS installer** - http://nodejs.org/

2. **Install the Grunt CLI (Command-Line Interface)**
    Open Applications/Utilities/Terminal.app and paste the following code, then hit enter.

    `npm install -g grunt-cli`

[Full Instructions Here](http://gruntjs.com/getting-started)

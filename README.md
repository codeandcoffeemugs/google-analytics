This base WordPress plugin is offered by [The App Store](http://getwpapps.com/developers) for WordPress: 
a place for WordPress developers to promote, support, and get paid for their work. 

Our plugin architecture teaches you to split your plugins into two versions: 
a *lite* version (which you will use for promotion), and a *pro* edition (which you will sell). 
This blueprint shows you how.

Make sure to read the Getting Started guide below, and be off and running on your project
in less than 5 minutes!

## Getting Started

From now on, you'll be using Git to manage your source. 

### Prepare your computer

You'll need to setup [Git and your GitHub account](http://help.github.com/). 

### Create accounts to host your plugin

You'll want to consider registering your plugin's namespace on three different sites:

1. [wordpress.org](http://wordpress.org/extend/plugins/add/) - where you'll promote the *lite* version of your plugin

2. [github.com](https://github.com/repositories/new) - where you'll be hosting your source code (the *best* place to promote
   open source, especially when [required to do so](http://wordpress.org/extend/plugins/about/) 
   (refer to the part about being required to use a GPLv2-compatible license)
   
3. [getwpapps.com](http://getwpapps.com/developers) - Coming soon: where we hope you'll be selling the distribution of
   the pro version of your plugin, and supporting the community that forms around your awesome software!

### Clone your WordPress.org subversion repository

Did you know you can use Git to manage subversion repositories? Yes, you can!

    ~ #> git svn clone http:// <your-plugin> --username
    ~ #> cd <your-plugin>
    your-plugin #> git config --add svn-remote.tags.url http:// 
    your-plugin #> git config --add svn-remote.tags.fetch :refs/remotes/tags

### Connect our project to your subversion checkout

This will pull our plugin skeleton into your project.

    your-plugin #> git remote add wpapp git@github.com:collegeman/wpapp.git
    your-plugin #> git pull wpapp master
    
### Connect your GitHub project

Very important: your GitHub project should **not** be a fork of our own. You'll
want your plugins to have their own names. They shall be forks of this project in
*spirit* alone.

    your-plugin #> git remote add origin git@github.com:<username>/<your-plugin>.git
    your-plugin #> 

## Development



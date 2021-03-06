Useful-Tools
============

*Useful tools for frontend development*

##Table of Contents
- [IDE](#ide)
	- [Webstorm](#webstorm)
- [Markdown](#markdown)
- [Grunt](#grunt)
- [Duo](#duo)
- [Bower](#bower)
- [Wiredep](#wiredep)

#IDE
##Webstorm
Webstorm is a smart JS IDE, see http://www.jetbrains.com/webstorm/

##Markdown
Use github flavored markdown to write ```README.md``` file on github.

- [Markdown Syntax](https://guides.github.com/features/mastering-markdown/)

Use a visual editor to help you write beautiful doc quickly.

- [Markdown Editor](http://jbt.github.io/markdown-editor/)

Install the Markdown Here chrome plugin: 

https://chrome.google.com/webstore/detail/markdown-here/elifhakcjgalahccnjkneoccemfahfoa

##Grunt
Grunt is a tasker runner.For more infomation, please see http://gruntjs.com/

You can use Grunt to 

- Watch file changes, you can see changes by refresh the page in browser, no need to manually restart server any more! 
- Detect errors and potential problems in the code
- ...

####Set up guide for watching file changes

1. For first time use, you need to install grunt and grunt plugins, and save devDependencies into ```package.json``` file with command```--save-dev```. With these operations, you only need to run ```npm install``` to install dev packages later.
```
npm install grunt --save-dev
npm install grunt-develop --save-dev
npm install grunt-contrib-watch --save-dev
npm install time-grunt --save-dev
npm install load-grunt-tasks --save-dev
npm install request --save-dev
```
2. Add ```Gruntfile.js``` into project root directory
3. Start server use ```grunt```, instead of ```npm start```

####For detect JS syntax errors
Install jshint with command ```npm install grunt-contrib-jshint --save-dev```, dont' forget to modify configuation in ```Gruntfile.js```, for more details, please see [Set up grunt with jshint](http://fcfeibel.com/blog/2013/07/28/grunt-quickstart-set-up-grunt-with-jshint/)


##Duo 

Duo is a next-generation package manager that blends the best ideas from Component, Browserify and Go to make organizing and writing front-end code quick and painless.

http://duojs.org/ 


##Bower
Web sites are made of lots of things — frameworks, libraries, assets, utilities, and rainbows. Bower manages all these things for you.

http://bower.io/

####Tips
- use [wiredep](#wiredep) to inject your Bower dependencies right into your HTML.

##Wiredep
Wire Bower dependencies to your source code. For more details please see: https://github.com/taptapship/wiredep

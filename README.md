#pwfoundation5
**This is a dropin template for the fabulous Open Source CMS Processwire, using Zurb Foundation 5 Compass files.**

It is based on Ryan Cramers [FoundationSiteProfile](https://github.com/ryancramerdesign/FoundationSiteProfile).

This template integrates Foundation 5 nicely into Processwire. It produces only one CSS file (templates/styles/style.css) that contains all the Foundation CSS and the custom template styles.

To achieve this, the template works with Foundations Compass SCSS files.

It is aimed at users that are either familiar working with SASS/SCSS/Compass or want to learn it.

This is __NOT__ a template where you want to edit the style.css file directly.

---

The CSS output is highly customizable.

Everything CSS related happens in the **scss** folder.

To **configure** your **Foundation** output, you can modify **templates/scss/styles.scss** and **templates/scss/_settings.scss**

All the **project specific** styles can be found in **templates/scss/ui/_main.scss**.

You can define more scss files in the ui folder and then include them.
For example you could add */templates/scss/ui/_menu.scss* and then add the line

```@import "ui/menu"```

to *templates/scss/style.scss*.

To recompile simply open a terminal, go to yourproject/site/templates/scss and do `compass watch`.
There are other ways doing this with GUI apps. Since I prefer the commandline, I can't tell you more about it.

This way you have one scss module for the menu styling and don't have to go through a long css file to find the menu styles. That's just one advantage of SASS, for those who are new to the subject.

##Prerequisites
In order to use this template and compile the CSS from the SCSS files your machine needs the following software:

1. COMPASS (which needs Ruby). [See howto install](http://compass-style.org/install/)
2. ZURB Foundation Gem. [See how to do this](http://foundation.zurb.com/docs/v/4.3.2/sass.html)(section *"Working with Existing projects"*) or do `gem install zurb-foundation` in a terminal.

##Install the template to a fresh Processwire site

Method 1:

1. Download the [zip file from here](https://github.com/gebeer/pwfoundation5/archive/master.zip), unpack it.
2. Replace */site-default/templates* and *config.php* with the files you just unpacked.
3. Install PW

Method 2 (command line):

1. Go to your Processwires site-default folder and delete the folder *templates* and the file *config.php* 
2. Open a terminal in */site-default* and do `git clone https://github.com/gebeer/pwfoundation5.git`
3. Install PW

##Update Foundation
You can update the Foundation framework independently from your project by doing `[sudo] gem update zurb-foundation` at a command prompt. Then recompile your CSS and you should be fine.
There are some more options for updating at the [official Foundation Documentation](http://foundation.zurb.com/docs/v/4.3.2/sass.html)(see section "Upgrading Foundation Compass projects")


##Javascript
By default the template uses the *foundation.min.js* which includes all Foundation JS modules.

If you use only some of them you could include them individually. They all sit in templates/scripts/foundation.


##Contribute
This is a work in progress.
Everyone is welcome to fork it, change it to their liking and improve on it.
If you detect bugs, pull requests are welcome.

##Discussion
I share this with other Processwire users [at the forum](http://processwire.com/talk/topic/5293-zurb-foundation-5-profiles/#entry51707). If you have questions, post them there. I will try and answer them.

##Last note about OS
I'm working on a linux box. Installation instructions for Ruby/Compass/Foundation gem should be fairly identical on Mac OSX. Windows users: sorry, I don't know. But I guess there are ways to do this on Windows. Your favorite searchengine might be helpful...

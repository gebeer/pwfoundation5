#pwfoundation5
**This is a dropin template for the fabulous Open Source CMS Processwire, using Zurb Foundation 5 Compass files.**

It is based on Ryan Cramers [FoundationSiteProfile](https://github.com/ryancramerdesign/FoundationSiteProfile).

This template integrates Foundation 5 nicely into Processwire. It produces only one CSS file (styles/style.css) that conatins all the Foundation CSS and the custom template syles.

To achieve this, the template works with Foundations Compass SCSS files.

It is aimed at users that are either familiar working with SASS/SCSS/Compass or want to learn it.

This is __NOT__ a template where you want to edit the style.css file directly.

---

The CSS output is highly customizable.

Everything CSS related happens in the **scss** folder.

To **configure** your **Foundation** output, you can modify **scss/styles.scss** and **scss/_settings.scss**

All the **project specific** styles can be found in **scss/ui/_main.scss**.

You can define more scss files in the ui folder and then include them.
For example you could add */scss/ui/_menu.scss* and then add the line

```@import "ui/menu"```

to *scss/styles.scss*.

This way you have one scss module for the menu styling and don't have to go through a long css file to find the menu styles. That's just one advantage of SASS, for those who are new to the subject.

##Prerequisites
In order to use this template and compile the CSS from the SCSS files your machine needs the following software:
1. COMPASS (which needs Ruby). [See howto install](http://compass-style.org/install/)
2. ZURB Foundation Gem. [See how to do this](http://foundation.zurb.com/docs/v/4.3.2/sass.html)(section *"Working with Existing projects"*) or do `gem install zurb-foundation` in a terminal.

##Install the template
Either download the zip file from here

CSS-On-Diet - easy and fast CSS preprocessor
============================================

This is [CSS-On-Diet](http://cssondiet.com) package for Sublime Text v2 and v3 for Mac, Linux and Windows. 
[CSS-On-Diet](http://cssondiet.com) is a preprocessor. It works like [Emmet](http://emmet.io/), but on the CSS level.  

![screenshot](https://raw.github.com/wyderkat/css-on-diet--sublime-text/master/screenshot.gif)

This package includes:

1.  Syntax highlighter
2.  Build system
3.  The preprocessor itself!

Installation
============

Package Manager
---------------
You can install via [Sublime Package Control](http://wbond.net/sublime_packages/package_control)

Manual
------
Or you can clone [this repo](https://github.com/wyderkat/css-on-diet--sublime-text) into your *Sublime Text [2|3]/Packages* directory

Preprocessor included
---------------------
Because CSS-On-Diet preprocessor is included in this package you don't have to install it separately. But you can do it. It will be favor over included one.

CSS-On-Diet quick documentation
===============================

CSS-On-Diet is a preprocessor for CSS files. The key feature is mnemonics for frequently used properties, which are similar to Emmet abbreviations. Other goodies include intuitive media breakpoints, nested and single line comments, variables and mixins, a calculator, hexadecimal RGBA, minifier, ...

Use old CSS
-----------

    .element {
      letter-spacing: 2px;
      background-color: #1C6BA0;
    }

If all your CSS declarations are on separate lines you don't have to change anything

Remove colons
-------------

    .element {
      letter-spacing 2px
      background-color #1C6BA0
    }

In CSS-On-Diet colons and semicolons are optional

Use mnemonics
-------------

    .element {
      les 2p
      bac #1C6BA0
    }

Common CSS keywords have mnemonics. Parameters are 3 letters long, values 2, and units just 1 letter ([The list](http://cssondiet.com/specification))

Medias Breakpoints
------------------

    @cod-media {
      tablet (min-width: 768px)
    }
    .element {
      les 2p
      les 3p @tablet
    }

Responsive Web Design was never so easy and intuitive

One line comments
-----------------

    .element {
      les 2p // why not 3?
      bac #1C6BA0 // deep ocean
    }

No need to remember to close those comments

Nested comments
---------------

    .element {
      /*
      les /*3p*/ 2p
      */
      bac #1C6BA0
    }

Now you can comment out code with other comment inside. Finally...
 
Arithmetics
-----------

    .element {
      les 3p-1
      bac #1C6BA0
    }

CSS needs calculations. That's more than sure.

Short RGBA
----------

    .element {
      les 3p-1
      bac #1C6BA0F1
    }

Just two more digits and you have transparency with your color

Variables
---------

    @cod-defines {
      sp2014 3p-1
      ocean #1C6BA0F1
    }
    .element {
      les sp2014
      bac ocean
    }

Defines are like variables. Write it once and use it anywhere. Stay DRY!

Mixins
------

    @cod-defines {
      sp2014 3p-1
      ocean bac #1C6BA0_ARG1_ ;\
            bai url("fish.png")
    }
    .element {
      les sp2014
      ocean(F1)
    }

Mixins can be anything placed anywhere. Arguments give them programming power.

More info at [CSS-On-Diet page](http://cssondiet.com)

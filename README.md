CSS-On-Diet - easy and fast CSS preprocessor
============================================

This is [CSS-On-Diet](http://www.cofoh.com/css-on-diet) package for 
Sublime Text v2 and v3 for Mac, Linux and Windows. 
[CSS-On-Diet](http://www.cofoh.com/css-on-diet) is a preprocessor. It works
like [Emmet](http://emmet.io/), but on the CSS level.  

![screenshot](https://raw.github.com/wyderkat/css-on-diet--sublime-text/master/screenshot.png)

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

CSS-On-Diet is a preprocessor for CSS files. The key feature are mnemonics for frequently used properties and value names, which are similar to Emmet abbreviations. Other goodies include optional colons and semicolons, nested and one line comments, variables and mixins, calculator, hexadecimal RGBA.

Use old CSS
-----------

    .element {
      letter-spacing: 2px;
      background-color: #1C6BA0;
    }

If all your CSS declarations are in separate lines you don't have to change anything. Normal CSS can be mixed with CSS-On-Diet.

Remove colons
-------------

    .element {
      letter-spacing 2px
      background-color #1C6BA0
    }

In CSS-On-Diet colons and semicolons are optional.

Use mnemonics
-------------

    .element {
      les 2p
      bac #1C6BA0
    }

Common CSS keywords have mnemonics. Parameters are 3 letters long, values 2, and units just 1 letter ([The list](http://www.cofoh.com/css-on-diet-1.1))

One line comments
-----------------

    .element {
      les 2p // why not 3?
      bac #1C6BA0 // deep ocean
    }

One line comments finish at the end of the line. No need to close it anymore.

Nested comments
---------------

    .element {
      /*
      les /*3p*/ 2p
      */
      bac #1C6BA0
    }

Now you can comment out code with other comment. Finally...

Arithmetics
-----------

    .element {
      les 3p-1
      bac #1C6BA0
    }

CSS doesn't need complicated calculations. But it needs some basic operations.

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
      ocean #1C6BA0_ARG1_
    }
    .element {
      les sp2014
      bac ocean(F1)
    }

Mixins are defines with arguments. Easy to use but powerful syntax.


RESPONSIVE MENUS
===================

Responsify your menus! Just give me a CSS or jQuery style selector
of your menu and I will make it mobile friendly (when the time is right).

CONTENTS OF THIS FILE
---------------------

 - Introduction
 - Tested
 - Known Issues
 - Special Thanks
 - Requirements
 - Installation
 - Coming From Drupal?
 - Usage
 - License
 - Credits
 - Maintainers

TESTED
-----

Working in Backdrop 1.1
Mainly tested to fit Seven and contrib themes rather than Bartik theme.

KNOWN ISSUES
---------------------

Some of the menu styles require Libraries module and downloading third-party plugins to the libraries folder as indicated in the settings page.

The Multi-Level Push Menu style does not work very well out of the box but the maintainer is pressed for time so you will have to spend a little time writing CSS to make it how you want if you want to use this style.

Upon installing, there will be an error message for checking if Backdrop has the right version of JQuery is installed.  This is a false check -- do not worry about it, and once you select your style the message will go away.  The maintainer is pressed for time so if you would like to fix this you are welcome to.

This hasn't been tested with every available option and every available theme, so you might find a conflict somewhere.  Let us know and we will fix it.

SPECIAL THANKS
--------------

https://drupal.org/user/433663 for this nice module


REQUIREMENTS
------------

menu and block modules enabled.

INSTALLATION
------------

Install this module using the official Backdrop CMS instructions at https://backdropcms.org/guide/modules

COMING FROM DRUPAL?
-------------------

A basic desktop CSS only dropdown menu option for screen width 769+ is available and will be worked on.  You may choose to write your own CSS to style this how you want.

PERMISSIONS
------------

@todo


USAGE
------------
For many use cases, the default settings will be enough.  Turn it on = done.
I am a huge fan of 0-config, too many things to configure in Backdrop already.
That said, there are plenty of configuration options at:
/admin/config/user-interface/responsive_menus

These options vary depending on the style chosen, but may include:
-CSS/jQuery selectors for which menus to responsify
-Text or HTML to use as the menu toggle button
-Screen width to respond to
-Open from Left or Right side of screen
-Remove other classes/id's when responded


GOOD TO KNOW
------------
The 'Simple' and 'MeanMenu' styles are included with this module, the others must be downloaded.  The URL to download a library will be presented to you if you try to choose any other style.

Sidr & codrops integrate with the Libraries module in order to work.
-This can be bypassed using hook_responsive_menus_styles_alter.
-See API & HOOKS below.

Google Nexus style takes over all the time (not just small screen).
-May be updated later to have a mobile only option.


API & HOOKS
-----------
hook_responsive_menus_style_info()
- Declare your own style.
hook_responsive_menus_styles_alter(&$styles)
- Alter existing styles.
@see responsive_menus.api.php

LICENSE
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for complete text.

CREDITS
-----------

- drastik <https://drupal.org/user/433663>
<http://drastikbydesign.com>

MAINTAINERS
-----------

 - biolithic <https://github.com/biolithic>

Ported to Backdrop by:

 - biolithic <https://github.com/biolithic>

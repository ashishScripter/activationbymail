## Introduction ##

Current state of the module is not giving you ability to modify views and e-mails presented to the customer from administration panel. Those features may be added in the future but currently they are not available, however it does not mean that you can not modify this content. Below are some cases and instruction for modifying some parts of the module to match your needs.


## Modifying overview ##

The newest version of the module is rewritten so it uses newest API supplied by Prestashop 1.5.x. That means that module is more MVC compatible than previous versions. This page is written from perspective of the newest version, prevision version can also be modified but location of some files may be different, however same rules applies when trying to do customization.

## How to edit files ##

You can edit files locally after extracting distribution package or remotely by ssh using vim or other text editor. When editing files locally remember to upload them after edit&save operation. You can also search for other software that allows you to edit text files on remote server.


## Files extensions important from customization point of view ##

  * .tpl - view files for Smarty Engine, basically they are html files with content holders
  * .html - pure html files, used for mails, may have some content holders
  * .txt - text files, used for mails, may have some content holders
  * other files types - should not be modified


## Mods ##

### Mod: Info for registered user ###

This is the information that informs customer that his account was created but it is not activated and corresponding mail will be sent to his e-mail address:

File: views/templates/front/info.tpl


### Mod: Activation successful ###

This is the information showed to the user after clicking link in the mail and after account was successfully activated.

File: views/templates/front/activation-success.tpl


### Mod: Activation failed ###

This is the information showed to the user after clicking link in the mail and after account was not successfully activated.

File: views/templates/front/activation-fail.tpl


### Mod: Mails ###

Mails are kept in multilanguage friendly structure. Message is presented as html file or txt file, when changing content in one file you must remember to change content in second file. When editing, do not remove content holders.

ISO\_CODE: en, pl

File: mails/ISO\_CODE/account\_activation.html

File: mails/ISO\_CODE/account\_activation.txt
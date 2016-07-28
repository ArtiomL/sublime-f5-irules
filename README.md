# <img align="center" src="Icons/sublime.ico" height="72">&nbsp;&nbsp;sublime-f5-irules
[![Releases](https://img.shields.io/github/release/ArtiomL/sublime-f5-irules.svg)](https://github.com/ArtiomL/sublime-f5-irules/releases)
[![Commits](https://img.shields.io/github/commits-since/ArtiomL/sublime-f5-irules/v12.1.1.svg?label=commits%20since)](https://github.com/ArtiomL/sublime-f5-irules/commits/master)
[![Maintenance](https://img.shields.io/maintenance/yes/2016.svg)](https://github.com/ArtiomL/sublime-f5-irules/graphs/code-frequency)
[![Issues](https://img.shields.io/github/issues/ArtiomL/sublime-f5-irules.svg)](https://github.com/ArtiomL/sublime-f5-irules/issues)
[![Sublime Text](https://img.shields.io/badge/sublime%20text-3114-orange.svg)](https://www.sublimetext.com/3)
![TMOS](https://img.shields.io/badge/tmos-12.1-ff0000.svg)
[![Package Control](https://img.shields.io/packagecontrol/dt/F5%20iRules.svg)](https://packagecontrol.io/packages/F5%20iRules)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)
<br>
## Description

Sublime Text package for F5 iRules syntax highlighting and auto-completion.

<br>
## Installation
#### [Package Control](https://packagecontrol.io/packages/F5%20iRules)
This is the recommended way to install the package. Package Control will install the latest release on your system and keep it up to date:

* Make sure Package Control is [installed](https://packagecontrol.io/installation)
* Open the **_Command Palette_** from the main menu of Sublime Text (Tools → Command Palette or ⌘+⇧+P)
* Start typing: `Package Control: Install Package` and select the command to show a list of all available packages
* Type: `F5 iRules` and select it to install the package

#### Manual (Windows, Linux, macOS)

* [Download](https://github.com/ArtiomL/sublime-f5-irules/archive/master.zip) the **master** branch archive
* Open the **_Packages_** directory from the main menu of Sublime Text (Preferences → Browse Packages...)
* Extract the archive into its own folder under the _Packages_ directory

#### Git
> Linux:

```
cd ~/.config/sublime-text-3/Packages
git clone https://github.com/ArtiomL/sublime-f5-irules.git
```

> macOS:

```
cd ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/
git clone https://github.com/ArtiomL/sublime-f5-irules.git
```

<br>
## Color Scheme
Please use the **_MonokaiRule_** theme included in this package for optimal highlighting experience.

<br>
## Filetypes and Syntax Association
The package syntax is used for ```.irule``` files by default.

Using the ```.txt``` extension is also supported: the first line of the file should begin with the following sequence:

```
#!iRule
```

Or you can set the syntax manually:

* Open the **_Command Palette_** from the main menu of Sublime Text (Tools → Command Palette or ⌘+⇧+P)
* Start typing: `Set Syntax: iRule` or `ssir` and select the command to activate it

<br>
## Snippets
Code snippets are small blocks of reusable code that can be inserted into a file to avoid repetitive typing.
Start typing one of the following:
```
for
foreach
if
switch
when
```

<br>
## Pseudo-Validation
Highlighting for a specific scope will be disabled (to indicate an **_error_**) based on the following set of rules:
#### Spaces
- Only a single space should be used between the highlighted commands, arguments and operators

#### Events
- The **_when_** statement can't start with a whitespace
- Only a single space should be used between the **_when_** keyword and the **_EVENT_NAME_**
- The **_EVENT_NAME_** should only contain capital letters, underscores and numeral 2<br>(for _ACCESS2_POLICY_EXPRESSION_EVAL_)

#### More
- In development

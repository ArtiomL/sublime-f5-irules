# <img align="center" src="Icons/sublime.ico" height="72">&nbsp;&nbsp;sublime-f5-irules
[![Releases](https://img.shields.io/github/release/ArtiomL/sublime-f5-irules.svg)](https://github.com/ArtiomL/sublime-f5-irules/releases)
[![Maintenance](https://img.shields.io/maintenance/yes/2016.svg)](https://github.com/ArtiomL/sublime-f5-irules/graphs/code-frequency)
[![Commits](https://img.shields.io/github/commits-since/ArtiomL/sublime-f5-irules/v12.1.0.svg)](https://github.com/ArtiomL/sublime-f5-irules/graphs/commit-activity)
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
#### Package Control
This is the recommended way to install the package. Package Control will install the latest release on your system and keep it up to date.
* Make sure Package Control is [installed](https://packagecontrol.io/installation)
* Open the **_Command Palette_** from the main menu of Sublime Text (Tools → Command Palette)
* Start typing: `Package Control: Install Package`
* Type: `F5 iRules` and select it to install

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

<br>
## Pseudo-Validation
Highlighting for a specific scope will be disabled (to indicate an **_error_**) based on the following set of rules:
#### Events
- The **_when_** statement can't start with a whitespace
- Only a single space should be used between the **_when_** keyword and the **_EVENT_NAME_**
- The **_EVENT_NAME_** should only contain capital letters, underscores and numeral 2<br>(for _ACCESS2_POLICY_EXPRESSION_EVAL_)

#### Log
- Only a single space should be used between the **_log_** command and its arguments: **_[-noname] \<facility\>._**

# SAS language support in Atom [![Build Status](https://travis-ci.org/akanosora/language-sas.svg?branch=master)](https://travis-ci.org/akanosora/language-sas)

Adds syntax highlighting, auto indentation, and snippets to SAS and SAS macro files in Atom.

In the past a few years, I have been mainly using Vim to code my SAS programs. I recently decided to switch to Atom for its better integration with OS X. This SAS language package is my first effort to switch to the new editor. I wrote the Vim SAS [syntax script](http://www.vim.org/scripts/script.php?script_id=3522) and [indentation script](http://www.vim.org/scripts/script.php?script_id=4034) and I feel that Atom allows me to better implement what I did in Vim.

Contributions are greatly appreciated. Please fork this repository and open a pull request to add modifications.

## Features

### Syntax highlighting

Syntax highlighting supports base SAS syntaxes up to **SAS 9.3**. It can automatically distinguish different statement keywords with respect to **data step** and **procedure** sections. This package also supports highlighting the specific **SQL** procedure keywords.

![Syntax highlighting](https://cloud.githubusercontent.com/assets/9272721/6994373/a32ed9e8-dadc-11e4-9e5b-a1a82bfc19cc.png)
> The screenshot used the default One Dark theme.

### Auto indentation

Just like syntax highlighting, it is completely rewritten. However, there are some limitations due to how Atom currently implements its indentation mechanism. I was not able to implement the exact indentation behavior as what I did in the Vim SAS indentation script. Right now, please make sure to use `run;` or `quit;` to close **data step** and **procedure** sections.

### Snippets

The following snippets are supported:

* `if` statement: `if`, `elsif`, `else`
* `do` statement: `do`, `while`, `until`
* `select` statement: `select`
* Array: `array`
* File input: `infile`
* Hash declaration: `declare`
* Procedure: `proc`
* FREQ - `tables` statement: `table`
* SQL - create table: `create`


## Install

Go to `Atom > Preferences...` then search for **SAS Language** in Install tab.

## To-Do List

* ~~Snippets~~
* SAS/STAT syntax highlighting
* PROC IML specific syntax highlighting
* Improve indentation mechanism?

## Copyright & License

Copyright ® 2015 Zhen-Huan Hu. This package is licensed under the MIT license.

SAS and all other SAS Institute Inc. product or service names are registered trademarks or trademarks of
SAS Institute Inc. in the USA and other countries.

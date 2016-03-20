# find-namespace-php

This PHP CLI software simplifies searching and finding class names and interface's Namespaces.

## Installation - manual
Copy the raw contents of the fns file and place it in your software/framework root folder.
Run it by opening a terminal and executing `php fns`

## Installation - composer
Add `carlhannes/find-namespace-php` to your composer.json
```js
"require": {
    "carlhannes/find-namespace-php": "*"
}
```
Run it by opening a terminal and using `php vendor/carlhannes/find-namespace-php/fns`,
it should find out your working directory by default. Otherwise you can use CD.

## Usage
When running, it will start an interactive shell where you can search for classes.
Type help for a complete list of commands. 

* `cd <path>` change current working directory (when no path, same as `pwd`)
* `clear` clear the screen (shorthandles: `cls`)
* `copy <index>` copy an item after using `find` (shorthandles: `c`, `get`, `g`)
* `config` to view the current configuration (shorthandles: `cfg`)
* `exit` to exit the application (shorthandles: `quit`, `end`, `q`)
* `find <search>` to search for a class or interface with a namespace (shorthandles: `f`)
* `help` list commands
* `list` list all FQCNS (shorthandles: `l`)
* `ls` list items in current directory (shorthandles: `dir`)
* `pwd` show the full path of the current working directory
* `reload` reload the cache/db (shorthandles: `r`)
* `toggle <var>` toggle a var from `config` on or off (shorthandles: `t`)

## Example
```
php fns
laravel fns > find view
Array
(
   [0] => Illuminate\Foundation\Console\ViewPublishCommand
   [1] => Illuminate\Foundation\ViewPublisher
   [2] => Illuminate\Support\Facades\View
)
laravel fns > copy 2 
Illuminate\Support\Facades\View copied to clipboard
```
## Tips 
Add `.fns.data.json` to your `.gitignore` file

Created by https://github.com/carlhannes
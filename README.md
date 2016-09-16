vim-autosave
============
> A plugin to automatically save your files

This plugin uses timers to automatically save your work as temporary files.

This makes use of the new timer functionality available with Vim 8.
Backup files will be written (by default every 5 minutes if the buffer was changed)
in your `backupdir` setting with a default extensions of '.backup' 

Installation
---

Use the plugin manager of your choice.

Alternatively, since Vim 8 includes a package manager by default, clone this repository below
`~/.vim/pack/dist/start/`

You should have a directory `~/.vim/pack/dist/start/vim-autosave`
That directory will be loaded automatically by Vim.

Usage
---
Once installed, take a look at the help at `:h vim-autosave` (not yet available).

Here is a short overview of the functionality provided by the plugin:
####Ex commands:
    :EnableAutoSave     - Enable the plugin (by default every 5 minutes)
    :DisableAutoSave    - Disable the plugin
    :AutoSave <millis>  - Enable the plugin (every <millis> milliseconds)
    :AutoSave           - Output status of the plugin

####Configuration variables (and defaults)
    :let g:autosave_extensions = '.backup'  - extension used for saving modified files
    :let g:autosave_timer      = 60*5*1000  - number of milliseconds to trigger
                                              (by default every 5 minutes)

License & Copyright
-------

Developed by Christian Brabandt. 
The Vim License applies. See `:h license`

© 2009-2016 by Christian Brabandt

__NO WARRANTY, EXPRESS OR IMPLIED.  USE AT-YOUR-OWN-RISK__

The IronYard Laptop
======

Laptop is a script to set up a Mac OS X or Linux laptop for Rails development.

Requirements
------------

### Mac OS X - Install a C compiler:

1. For Mavericks (10.9): run `sudo xcodebuild -license` and follow the instructions
to accept the XCode agreement.  
1. Then run `xcode-select --install` in your terminal and then click "Install".

Install
-------

### Mac OS X

Run the script:

    bash <(curl -s https://raw.githubusercontent.com/tiy-houston-q3-rails/laptop/master/mac)


What it sets up
---------------

* Zsh as your shell
* Bundler gem for managing Ruby libraries
* Exuberant Ctags for indexing files for vim tab completion
* Foreman gem for serving Rails apps locally
* Heroku Config plugin for local `ENV` variables
* Heroku Toolbelt for interacting with the Heroku API
* Hub gem for interacting with the GitHub API
* Homebrew for managing operating system libraries (OS X only)
* ImageMagick for cropping and resizing images
* Postgres for storing relational data
* Qt for headless JavaScript testing via Capybara Webkit
* Rails gem for writing web applications
* Rbenv for managing versions of the Ruby programming language
* Redis for storing key-value data
* Ruby Build for installing Rubies
* Ruby stable for writing general-purpose code
* The Silver Searcher for finding things in files
* Tmux for saving project state and switching between projects
* Watch for periodically executing a program and displaying the output

It should take less than 15 minutes to install (depends on your machine).

Make your own customizations
----------------------------

Put your customizations in `~/.laptop.local`. For example, your
`~/.laptop.local` might look like this:

    #!/bin/sh

    brew tap phinze/homebrew-cask
    brew install brew-cask

    brew cask install dropbox
    brew cask install google-chrome
    brew cask install rdio


Credits
-------

![thoughtbot](http://thoughtbot.com/assets/tm/logo.png)

Laptop is maintained and funded by [thoughtbot, inc](http://thoughtbot.com/community).
The names and logos for thoughtbot are trademarks of thoughtbot, inc.

Thank you, [contributors](https://github.com/thoughtbot/laptop/graphs/contributors)!

Contributing
------------

Please see [CONTRIBUTING.md](https://github.com/thoughtbot/laptop/blob/master/CONTRIBUTING.md).

License
-------

Laptop is © 2011-2014 thoughtbot, inc. It is free software, and may be
redistributed under the terms specified in the LICENSE file.

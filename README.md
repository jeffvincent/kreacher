Kreacher
========

[Kreacher](http://harrypotter.wikia.com/wiki/Kreacher), is a script to set up a Mac OS X laptop for Wistia development.

Much of what follows is based on [Laptop](https://github.com/thoughtbot/laptop), a similar installer devised by the awesome folks at [Thoughtbot](http://thoughtbot.com/).

First Steps
------------

1) Install XCode, and the Command Line Tools for Xcode [more info](http://www.moncefbelyamani.com/how-to-install-xcode-homebrew-git-rvm-ruby-on-mac/)

2) While that is installing, [download iTerm2](http://iterm2.com).

3) Because it takes [FOREVER](http://www.youtube.com/watch?v=H-Q7b-vHY3Q) to download Xcode, you might as well also [create a GitHub account](https://github.com/). 
(We will order Kreacher to install Git for you)

4) Open iTerm2, and Set zsh as your login shell. (After running command, close and re-open iTerm2)

    chsh -s /bin/zsh

To Order Kreacher to do your bidding
------------------------------------

Run the script:

    zsh < <(curl -s https://raw.github.com/jeffvincent/kreacher/master/build)

What Kreacher will retrieve for you
-----------------------------------

* Ack for finding things in files
* Bundler gem for managing Ruby libraries
* Foreman gem for serving Rails apps locally
* Homebrew for managing operating system libraries
* Postgres for storing relational data
* Postgres gem for talking to Postgres from Ruby
* MySQL, for...MySQLing
* Rails gem for writing web applications
* Ruby stable for writing general-purpose code
* RVM for managing versions of the Ruby programming language
* Git, for tracking project versions efficiently
* SSH public key for authenticating with Github and Heroku
* Tmux for saving project state and switching between projects

It should take less than 15 minutes to install (depends on your machine).

Post Install
------------

    $ brew doctor

Other Notes
-----------

To run doomcrank, you will need to install Ruby 1.8.7 (pending update). Follow the instructions in [this post](http://stackoverflow.com/questions/11664835/mountain-lion-rvm-install-1-8-7-x11-error) for the fix.
If you have any trouble with cacerts, try: https://github.com/mxcl/homebrew/issues/6103#issuecomment-1694558

Credits
-------

![thoughtbot](http://thoughtbot.com/images/tm/logo.png)

So so much of this is based on Laptop by [thoughtbot, inc](http://thoughtbot.com/community).
The names and logos for thoughtbot are trademarks of thoughtbot, inc.

Thank you to their [contributors](/thoughtbot/laptop/graphs/contributors)!

License
-------

Because Typhon is heavily based on Laptop, seems right to use their license I think.

Laptop is © 2011-2012 thoughtbot, inc. It is free software, and may be
redistributed under the terms specified in the LICENSE file.

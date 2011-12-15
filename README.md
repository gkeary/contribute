RubyGems Developers
===================

Showing off the latest and greatest projects in the RubyGems ecosystem!

Goals
=====

* Help developers get involved in RubyGems and its associated projects
* Have one place to find out where these projects are!

Setup
=====

This is a Rails 3.1 app that is deployed to Heroku. Get the app running on your box with:

    bundle
    rails server

Done! There's no database requirement (in fact, ActiveRecord is not loaded at all!) so setup should go smoothly.

Setup Note: A JavaScript runtime is required
===============================

On Linux, Rails 3.1 requires a JavaScript runtime.  

When Rails can't find one, it throws the following 
exception message: 


    Linux Could not find a JavaScript runtime.  
    See https://github.com/sstephenson/execjs 
    for a list of available runtimes.  
    (ExecJS::RuntimeUnavailable)

To fix this error either install node.js with:
    sudo apt-get nodejs

OR

Include 'therubyracer' in your Gemfile.

To use the ruby racer in rails, or any application using Bundler to manage gems, add the following to your Gemfile

   gem "therubyracer", :require => 'v8'
   gem "therubyracer", "~> 0.8.2.pre" #bleeding edge.

Adding links
============

This site's content lives mostly in `app/views/pages/home.html.md`. Jump in and edit it, send a pull request, and we'll merge it in!

Thanks
======

Huge thanks to [thoughtbot](http//thoughtbot.com) whose [playbook](http://playbook.thoughtbot.com) these styles are based off of.

Legal
=====

The actual content of the articles is licensed under Creative Commons. The code that this project consists of is licensed under MIT.

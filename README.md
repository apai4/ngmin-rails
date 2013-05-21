ngmin-rails
===========

Use <https://github.com/btford/ngmin> in the Rails asset pipeline.

Installation
------------

Add this line to your application's Gemfile:

    gem 'ngmin-rails'

And then execute:

    $ bundle

That's it! ngmin-rails integrates seamlessly into the Rails asset pipeline; your JavaScript or CoffeeScript assets will automatically be run through the ngmin pre-minifier.

Versioning
----------

The ngmin-rails version number mirrors the version number for the version of ngmin that is bundled with it.

Hacking
-------

### Upgrading ngmin

The actual ngmin project is bundled into this gem via [Browserify](https://github.com/substack/node-browserify). You can update to the latest version of ngmin via Rake:

    rake ngmin:build

### Test Application

There is a Rails 3 application bundled in `example/` that you can use to test the asset pipeline integration. Don't forget to remove `tmp/cache/assets` after upgrading to the latest version of ngmin.

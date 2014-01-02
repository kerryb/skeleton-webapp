# Skeleton web app

A basic skeleton project for simple javascript web apps, using [coffeescript](http://coffeescript.org/), [sass](http://sass-lang.com/) and [haml](http://haml.info/).

Provides a [guard](http://guardgem.org/) config to automatically rebuild the app when any source file changes. There's also a simple rack config, to expose the (static) built app in `public` on [port 3000](http://localhost:3000) for development.

## Getting started

Assuming you have ruby and coffeescript installed:

    bundle
    rake start
    guard

If everything builds successfully, this should result in a [page](http://localhost:3000) with a tick icon and no error messages.

## Rake tasks

The following rake tasks are provied for convenience:

    rake clean    # Remove any temporary products
    rake clobber  # Remove any generated file
    rake default  # Create site in public directory
    rake start    # Start a simple thin server for files in public directory
    rake stop     # Stop the thin server

## Live reload

If you install the [LiveReload](http://livereload.com/) browser extension and enable it when viewing your app, the page will reload whenever any file changes.
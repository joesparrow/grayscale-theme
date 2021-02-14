Website for Mordor Fun Run
==========================

Based on the Jekyll theme forked from https://github.com/jeromelachaud/grayscale-theme.

# Install for the first time

This uses Jekyll which is wonderful, but unfortunately requires Ruby on a mac, which is not.

Install the xcode command line tools for your flavour of MacOS from: https://developer.apple.com/download/more/

Install rvm:

    curl -sSL https://get.rvm.io | bash -s

Install ruby:

    bash # to get your newly installed rvm
    rvm install 3.0.0

Clone:

    git clone git@github.com:joesparrow/mordorfunrun
    cd mordorfunrun

Run:

    touch Gemfile
    gem install eventmachine -- --with-openssl-dir=/usr/local/opt/openssl@1.1
    gem install bundler
    bundle add webrick
    bundle add jekyll --version '~>3.9.0'
    bundle install

# Develop

Clone:

    git clone git@github.com:joesparrow/mordorfunrun
    cd mordorfunrun
    bundle install

Run jekyll with:

    bundle exec jekyll serve --incremental --watch

See the site locally: http://127.0.0.1:4000/

Or on github pages: https://mordorfunrun.github.io/

Or via domain name: https://mordorfunrun.co.uk

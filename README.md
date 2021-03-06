
This is a Ruby wrapper for Teambox API.

Largely inspired by @jnunemaker's Twitter gem.
This is currently in development, and is missing many methods.

Get started
-------------------------------------------------------------------------------

First, install the *teambox-client* gem:

    gem install teambox-client

Now, run `irb -rubygems` and this snippet to get the list of activities:

    require 'teambox-client'
    httpauth = Teambox::HTTPAuth.new(your_username, your_password)
    client = Teambox::Base.new(httpauth)
    puts client.activities

By default, *teambox-client* will connect to the hosted service at [teambox.com](http://teambox.com/), optionally you can:

    Teambox::HTTPAuth.new(your_username, your_password, :api_endpoint => 'localhost:3000')

Examples
-------------------------------------------------------------------------------

First, create a file on $HOME/.teambox with these values:

    username: your_teambox_username_or_email
    password: password

See the examples directory.

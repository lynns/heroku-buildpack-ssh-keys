Heroku buildpack: Private SSH Keys
===================================

This buildpack uses a private SSH key exposed to the environment as `SSH_KEY` in order to download
later buildpacks and app dependencies via Git+SSH without embedding a password into the url.

Usage
-----

Example usage:

    $ heroku create --stack cedar --buildpack http://github.com/fs-webdev/heroku-buildpack-ssh-keys.git

    $ source
    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> Private SSH Keys app detected

TODO!
# hephaisto.github.io
Website

## Using the raspberry builds
The repository contains all builds of my software that is designed to be used on a raspberry pi.
All packages are built against raspbian stable.

To use the packages, run the following as root:

    echo "deb http://hephaisto.github.io/raspbian_repository/ stable main" >> /etc/apt/sources.list
    wget -O - http://hephaisto.github.io/keys/buildservice.gpg.key | apt-key add -

Note: Of course you should not blindly download and install public keys. You should only do the above if you have verified my key or if you are myself ;)

After that, you can use the normal `apt-get update`/`apt-get install` commands.

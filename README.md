# Mumbletune

MUMBLETUNE is a nice bot that connects to a mumble server and allows users to listen to Spotify together.

This is my custom version, I will be adding a few extra features when i get the hang of ruby! :D

## Installation

What you need:
- A Spotify Premium account. I wish it didn't have to be this way, but for API access, Premium's required
- A Spotify App Key. Spotify will issue you one [here][1]. 

First, ensure you have some prerequisites (these commands are for Ubuntu 12.04, but should be similar on other Debian-based distributions. I have no experience running Mumbletune on Windows.)

    # Build tools (make, etc.), Git, and Ruby 1.9.3
    $ sudo apt-get install build-essential git ruby1.9.3 ruby-dev
    
    # CELT and libsamplerate
    $ sudo apt-get install libcelt-dev libsamplerate0-dev
    
    # Bundler
    $ gem install bundler

Then, clone Mumbletune and install its dependencies

    $ git clone git://github.com/elliottwilliams/mumbletune.git
    $ cd mumbletune
    $ bundle install

## Usage

1. Create a configuration file. See `conf.example.yaml` for help.
2. Start Mumbletune, passing your config with `-c`.

		$ mumbletune -c config_file.yaml

[1]: https://developer.spotify.com/technologies/libspotify/keys/

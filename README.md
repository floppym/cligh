# cligh - Command-line Interface to GitHub

This is a simple command-line interface to the facilities of GitHub.
It is written by Christopher Brannon <chris@the-brannons.com>.
The current version is 0.1.
This program is still in the early stage of development.
It is by no means feature-complete.
A friend and I consider it useful, but others may not.

## Obtaining

Obtain the current stable version using this link:
<http://the-brannons.com/software/cligh-0.1.tar.gz>.
You can verify the integrity of the file using the
[gpg signature](http://the-brannons.com/software/cligh-0.1.tar.gz.sig).

## Installation

If you are using a version of Python prior to 2.7, you first need to
install the argparse module.
Get it from [here](http://argparse.googlecode.com/).
Python version 2.7 includes argparse in its standard library.

cligh also requires the PyGithub package.
The homepage for PyGithub is [https://github.com/jacquev6/PyGithub](https://github.com/jacquev6/PyGithub).

The final dependency is PyXDG.
Get it from [http://freedesktop.org/Software/pyxdg](http://freedesktop.org/Software/pyxdg).

Once the dependencies are installed,
 type `./setup.py` in the cligh source directory, in order to install
the script.

## Setup

Run the following command to configure cligh:

    cligh configure

The program will prompt you for a username and password.  It then creates
an authorization using the Github API.
cligh never stores your password.  Instead, it stores the token associated
with the authorization that it created.
It uses this token to authenticate to Github.

## Usage

Usage is straightforward, and the program provides informative help
messages.  Simply type `cligh -h` at a shell prompt,
to see the introductory help message.

## Development

The source for this project is managed by git.  If you wish to contribute,
or if you simply wish to use the unpublished "development" sources, clone
it using a command such as the following:

    git clone git://github.com/CMB/cligh.git

Patches are most appreciated.  Please send them to [chris@the-brannons.com](mailto:chris@the-brannons.com).

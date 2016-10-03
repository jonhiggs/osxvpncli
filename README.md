# osxvpncli

This is a wrapper to help you start and stop your macOS VPN connections from the command line.

## Installation

The easiest method is via `homebrew`:

```ShellSession
    $ brew tap jonhiggs/homebrew-osxvpncli
    $ brew install osxvpncli
    $ osxvpncli --help
```

Alternatively you can just clone the git repository to your local system:

```ShellSession
    $ git clone https://github.com/jonhiggs/homebrew-osxvpncli.git <my_path>
    $ <my_path>/vpn --help
```

## Setup

Before you can do anything, you must first create the VPN connections that you wish to manipulate though `System Preferences -> Network`.

If you would like working tab-completion, you can use the completion script in `bash_completion.d/vpn`. If you're not sure how to use bash_completion scripts, take a look at [this blog post](http://blog.jeffterrace.com/2012/09/bash-completion-for-mac-os-x.html).

## Usage

    Usage:
      vpn [OPTION] [vpn_name]

    Options:
      connect     <vpn_name>  Establish a new connection
      disconnect  [vpn_name]  Terminate established connections
      status      [vpn_name]  Show connection status

## Change Log

## Version 0.2.2

- Rename `vpn` to `osxvpncli` to avoid being overly rude with naming.
- Document installation with `homebrew`.

## Version 0.2.1

- Disconnect all if connection isn't supplied. [#issue 5](https://github.com/jonhiggs/osxvpncli/issues/5)

## Version 0.2

- Remove support for OS X Yosemite.
- Refactor for simpler code

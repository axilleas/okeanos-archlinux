# Archlinux pkgbuilds for the [Okeanos IaaS] (https://okeanos.grnet.gr/welcome/).

##Installation

Use your favourite pacman wrapper to download and/or install `kamaki`
and `snf-image-creator` from AUR.

- [snf-image-creator](https://aur.archlinux.org/packages/snf-image-creator/)
- [kamaki](https://aur.archlinux.org/packages/kamaki)


## snf-image-creator

See http://docs.dev.grnet.gr/snf-image-creator/latest/index.html for more
information.

## ./kamaki

###kamakirc
If you own an account at okeanos, remeber to copy `kamakirc` to `$HOME/.kamakirc`
and place your API key to global configuration.

###Example
#### Rebooting a server
By invoking 

    $ kamaki server list

we get a list of our available servers. Let's say we have two of them:

    2800 ftpbackup
    2801 webserver

With the following command we reboot our `ftpbackup` with key-id `2800`:

    $ kamaki server reboot 2800


# CJDNS DUMPWEB #

## About ##

The behaviour of this script is simple: It uses `cjdcmd` to access the `cjdroute` admin port and dump the current routing table, parsing for ipv6 addresses, then iterates through each address and tests port 80, which it dumps to stdout when it receives a reply.

Simple parsers, robots etc. can use this to facilitate pulling data from Hyperboria.

## Requirements ##

 * **[cjdcmd](https://github.com/inhies/cjdcmd)**: Follow the [installation instructions](https://github.com/inhies/cjdcmd#installation) making sure it's available in `$PATH` and can successfully run `cjdcmd dump` by the time you're done.
 * **bash** and **wget**: The shell this script is being run from doesn't need to be `bash`, but it and `wget` need to be available in `$PATH`.

## Usage ##

Once `cjdcmd` is installed and working, the cjdns dumpweb script simply needs to be run from the commandline: `sh cjdns-dumpweb`.

## Credits ##

Written by Kevin MacMartin: [GitHub Projects](https://github.com/prurigro) | [Arch Linux AUR Packages](https://aur.archlinux.org/packages/?SeB=m&K=prurigro)

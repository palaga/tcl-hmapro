tcl-hmapro
==========

A tcl version of the hma shell script, to connect to their vpn server.

This script can be used as a replacement for the hma-vpn.sh script. This script
is still in an early stage of development. For a short help message, run it with
either no arguments or -h.

Configuration is pretty simple, with a _key_ = _value_ format. Comments start
with a #. A few examples of usage:

Show version:

  hmapro -v

Update server list and openvpn template:

  hmapro -u

List servers matching "Neth":

  hmapro -l Neth

Connect to first server of list matching "Neth":

  hmapro Neth

Same as previous line, but uses udp instead of tcp to connect:

  hmapro -p udp Neth

Use configuration file _example.cfg_:

  hmapro -c example.cfg Neth


Features
--------
- [x] Connect to a server.
- [x] List servers based on a regular expression.
- [x] Support for a configuration file.
- [ ] Enhanced configuration with formatable _vpncmd_ line.


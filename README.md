tcl-hmapro
==========

A tcl version of the hma shell script, to connect to their vpn server.

This script can be used as a replacement for the hma-vpn.sh script. This script
is still in an early stage of development. For a short help message, run it with
either no arguments or -h.

Configuration uses a safe tcl interpreter, with one added command: setcfg key
value. See the example.cfg file for some examples. A few examples of usage:

 ```sh
    $ hmapro -v                  # Show version
    $ hmapro -u                  # Update server list and openvpn template
    $ hmapro -l Neth             # List servers matching "Neth"
    $ hmapro Neth                # Connect to first server matching "Neth"
    $ hmapro -p udp Neth         # Use udp instead of tcp to connect
    $ hmapro -c example.cfg Neth # Use configuration file _example.cfg_
```


Features
--------
- Connect to a server.
- List servers based on a regular expression.
- Support for configuration files.


TODO
----
- Add a simple TK gui.


# ipv6-dhclient
Simple IPv6 configuration script for Debian-based and RedHat distros, mainly for [Online.net](http://www.online.net/) servers but valid for any network that provides IPv6 access through prefix delegation i.e. the static address is configured by the client and an identifier (DUID) is sent to the DHCP server in order to get functional routes.

Servers provided by [Online.net](http://www.online.net/) won't come with IPv6 enabled by default so this makes things a bit easier specially when owning multiple servers and IPv6 needs to be enabled by hand in each one.

The script has been successfully tested under:

* Ubuntu Server 14.04
* Debian 7.0
* CentOS 7.0

Just run the script and follow the instructions:

`$ bash ipv6-dhclient.sh`

You can also pass parameters straight away:

`$ bash ipv6-dhclient.sh <interface> <address block> <subnet> <duid>`

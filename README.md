# SipTest

SipTest is a simple tool to test some SIP messages. It is possible to send INVITE, REGISTER and OPTIONS.

```
$ perl siptest.pl 

SipTest - by Pepelux <pepeluxx@gmail.com>
-------

Usage: perl siptest.pl -h <host> [options]
 
== Options ==
-m  <string>     = Method: REGISTER/INVITE/OPTIONS (default: OPTIONS)
-u  <string>     = Username
-s  <integer>    = Source number (CallerID) (default: 100)
-d  <integer>    = Destination number (default: 100)
-r  <integer>    = Remote port (default: 5060)
-proto <string>  = Protocol (udp, tcp) - By default: UDP)
-ip <string>     = Source IP (by default it is the same as host)
-ua <string>     = Customize the UserAgent
-v               = Verbose (trace information)
 
== Examples ==
$perl siptest.pl -h 192.168.0.1
	To search SIP services on 192.168.0.1 port 5060 (using OPTIONS method)
$perl siptest.pl -h 192.168.0.1 -m INVITE
	To search SIP services on 192.168.0.1 port 5060 (using INVITE method)
```

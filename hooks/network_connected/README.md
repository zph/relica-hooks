# Summary

Script can be used as a pre-hook to verify that Relica's host is connected to a network where it should permit backups (ie wifi not mobile data).

Tested on OSX 10.14

# Usage

Install hook in reasonable location and make executable.

Setup a hook with:
```
Timing = Before each destination
On Error = Stop
Command = $HOME/bin/network_connected | grep 'MyWifi'
```

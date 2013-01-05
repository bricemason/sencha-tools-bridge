Sencha Tools Bridge
===================

A bash script to enable the Sencha SDK Tools for Sencha Touch 2.0 to 
co-exist with Sencha Cmd for Sencha Touch 2.1.

This script will not modify the Sencha SDK Tools or Sencha Cmd in any way. Instead it removes
Sencha SDK Tools and Sencha Cmd from the system PATH, then adds its containing
directory to the system PATH.

Once the bridge is installed, you can use the `sencha` command as you normally would. The bridge
will figure out the proper context and reroute the command to the correct toolset. 

Profile scripts `.bash_profile` and `.bashrc` are modified but backup copies are stored in
`.bash_profile.sencha-tools-bridge-save` and `.bashrc.sencha-tools-bridge-save` during both
the install and uninstall process.

This script has been tested on Mac OS X.

This project has absolutely no affiliation with Sencha.

Released under the MIT license. See LICENSE.md for details.

Requirements
-----------

- Sencha SDK Tools
- Sencha Cmd

Installation
------------

1. Download and extract the project
2. Make the bash script executable by issuing `chmod 755 ./sencha`
3. Install using command `./sencha install`
4. Issue `sencha` commands as you normally would

Uninstall
---------

1. Issue the command `sencha uninstall`

Contributions
-------------

The following people provided input via the Sencha forums:

- [mitchellsimoens](http://www.sencha.com/forum/member.php?22216-mitchellsimoens)
- [jweber](http://www.sencha.com/forum/member.php?502-jweber)

Forum posts:

- [SenchaCmd and SenchaSDKTools simultaneously?](http://www.sencha.com/forum/showthread.php?251810-SenchaCmd-and-SenchaSDKTools-simultaneously)
- [Sencha Tools Bridge - Using Sench SDK Tools with Sencha Cmd](http://www.sencha.com/forum/showthread.php?251862-Sencha-Tools-Bridge-Using-Sench-SDK-Tools-with-Sencha-Cmd)
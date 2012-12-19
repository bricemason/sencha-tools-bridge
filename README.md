Sencha Tools Bridge
===================

A bash script to enable the Sencha SDK Tools for Sencha Touch 2.0 to 
co-exist with Sencha Cmd for Sencha Touch 2.1.

This script will not modify the Sencha SDK Tools in any way. Instead it removes
Sencha SDK Tools from the system PATH, then adds a couple of symlinks to key resources
needed to run the tools. 

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
2. Make the bash script executable by issuing `chmod 755 sencha-bridge`
3. Install using command `sencha-bridge install pathToSDKTools` where *pathToSDKTools* is the path to the Sencha SDK Tools (not Sencha Cmd)

Once installation is complete, you will use the Sencha SDK Tools through the command `sencha-legacy`. 
Sencha Cmd can still be used by the command `sencha`.

For example, to generate a Sencha Touch 2.0 app:

    sencha-legacy generate app MyApp apps/my-app

To generate a Sencha Touch 2.1 app:

    sencha generate app MyApp apps/my-app

Uninstall
---------

1. Issue the command `sencha-bridge uninstall pathToSDKTools` where *pathToSDKTools* is the path to the Sencha SDK Tools (not Sencha Cmd)
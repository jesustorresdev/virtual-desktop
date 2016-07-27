virtual-desktop - Some scripts and configuration files of my virtual windows desktop with GPU passthrough.<br />
Copyright 2015-2016 Jesús Torres <jmtorres@ull.es>

## Installation

 1. Copy scritp
 2. Copy hook
 3. Copy configuration
 4. Copy sysctl.d

## Add a desktop shortcut

Create a desktop file (e.g. virtual-desktop.desktop) with the following content and put it in your desktop folder
or in ~/.local/share/applications, if you want to add it as a desktop menu entry.

~~~
[Desktop Entry]
Name=Virtual Desktop
GenericName=Windows virtual desktop launcher
Exec=/usr/local/bin/start-virtual-desktop --desktop hoth
Icon=virt-manager
Terminal=true
Type=Application
Categories=System;Office;Game
~~~

Remember change the Exec line so that it points to the path of `start-virtual-desktop` script. And replace
'hoth' with the name of your virtual machine.

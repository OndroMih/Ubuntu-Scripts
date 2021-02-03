# Ubuntu scripts

Scripts to automate small tasks. Designed for Ubuntu Focal 20.04 LTS. Some scripts require components used in Ubuntu (like Gnome Desktop), others are generali Linux scripts and should work in any Linux distribution.

## Desktop Zoom

A shell script to zoom screen in or out. Can be triggered on a key press or mouse scroll (e.g. using xbindkeys).

Requires:

* Gnome and DConf
* xdotool

Requires xbindkeys to bind to a mouse scroll wheel because Ubuntu Gnome doesn't support binding commands to mouse events, only to keyboard shortcuts.

## Disk cleanup

Scripts to clean up some disk space by deleting unnecessary files:


* `clean-maven-projects <path-to-the-root-directory-with-projects> [-f]` - deletes the generated `target` directories in maven projects
* `clean-docker-images` - deletes unused Docker images (either only dangling or all unused)

## Firewall

* `clean-firewall` - cleans all the firewall rules (sets the firewall to the vanilla configuration without any rules)

## Toggle touchpad

A script to enable/disable the touchpad. Can be bound to a keyboard shortcut. Useful if you accidentally touch the touchpad while writing on the keyboard and want to disable the touchpad while writing.

* `toggle-touchpad` - enables or disables the touchpad and pops up a system notification about the current status of the touchpad

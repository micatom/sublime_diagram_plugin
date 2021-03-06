# Why Fork

I forked the project to :
* allow persistence of the generated png file into a png surdir. 
* execute process in the file dir to make plantuml !include command works

# Overview

This is a plugin that renders diagrams from your selection in Sublime Text 2
or 3.

By default, it binds the (Command / Alt)-M key and registers a command on the
Command Palette.  Simple select the text for your diagram and trigger the
command.  Multiselections are allowed.  Each diagram will be generated in a
uniquely named file.

If a diagram handler recognizes a diagram in the selection, it will render it
and pop it up in a detected viewer.

If you wish to override the viewer used, create a user version of
Diagram.sublime-settings file in the usual way.


# Install

To install from scratch, it's necessary to have:

* Java (download from java.sun.com)
* Graphviz (I recommend "homebrew" on the Mac)
* Sublime Text 2 or 3


# Support

Operating Systems:  MacOS X, Linux
Diagram Types: PlantUML
Viewers (in order of preference):

* MacOS X Preview
* MacOS X QuickLook
* Eye of Gnome

Patches to support additional viewers or diagrams are welcome.

# Install Instructions

Check out the source directory or download and uncompress the source tarball.
Put this directoy in the Packages directory for your platform.

On Linux, it's sometimes "~/.config/sublime-text-2/Packages/".
On MacOS X, it's "~/Library/Application Support/Sublime Text 2/Packages/".

Sublime Text should detect the plugin and automatically load it.

The source is available via git at:

https://github.com/micatom/sublime_diagram_plugin.git

# Thanks

Special thanks to all of those who have contributed code and feedback,
including:

* Tobias Bielohlawek (Syntax Highlighting Support)
* Julian Godesa (UX feedback)
* Seán Labastille (Preview support, multi-diagram support)
* Kirk Strauser (Python 3 / SublimeText 3 Support)
* Stanislav Vitko (PlantUML updates)

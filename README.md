### Kingfish for Philips Hue, by Peter Kaminski

An open-source single-file HTML/JavaScript Hue controller for
interacting directly with the API. Intended for those who want to get
a better handle on the low-level interface to their Hue system.

You can load the `kingfish.html` file from this directory in your
browser, or load or save the file from the web:
[kingfish.html](http://peterkaminski.github.io/kingfish/kingfish.html).

Commands are sent on your local network directly from your device to
your Hue bridge, not through any server. (The "Get Bridge IP" command
retrieves your bridge IP address from a Philips server, but does not
send any data, nor does the Philips server send any commands.) There
are no analytics or tracking bugs in this file.

Start by doing boxes in numbered order, then repeat in any order as
desired. Green buttons set blue values, but don't send commands. Blue
and red buttons send commands to bridge. You can close and re-open
Kingfish at any time. Kingfish uses HTML5 local storage, if available
in your browser, to persist input values entered on your device.

Roadmap and other development ideas:

* XY color
* better mobile browser support
* graphical color picker
* Schedules and Rules, including sunrise/sunset+offset rules
* calendar/time picker
* Sensors
* using names of objects from bridge instead of numbers
* more attractive visually (better CSS)
* theming
* namespacing variables
* better code organization
* automatic parsing of responses
* countdown timer for monitoring transition time
* active programmatic control of lighting
  * bookmark colors, optionally name
  * randomly adjust colors (random walk, abrupt)
  * "bounce" light gently from lamp to lamp
* expand/close boxes
* drag-drop to rearrange boxes
* support for other similar systems

Kingfish uses [jQuery.ajax](http://api.jquery.com/jquery.ajax/) to
send commands via HTTP to the bridge. For background on Philips Hue
terminology and how the Hue API works, read [Philips hue
API](https://developers.meethue.com/develop/hue-api/). Visit the
[Kingfish project home page](http://peterkaminski.github.io/kingfish/)
or the [Kingfish repo](https://github.com/peterkaminski/kingfish) to
comment, fork, or download the project files. Distributed under
open-source MIT license, see LICENSE.md.

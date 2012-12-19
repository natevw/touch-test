# Browser touch events tester

This is a very barebones HTML5 utility that simply shows mouse/touch/pointer–related events, in both a log format and simple visual display of the interaction identifier.

For example, when I last tested:

* mainframe browsers normally just provide mouse down/move/up events
* iOS Safari, Nexus 7 (Chrome and Firefox) all provide touch events with multiple fingers
* my Kobo Touch's unsuported "extra" browser only delivers click (mouseup/down) events and no movement
* the Kindle Fire "Silk" browser sent touch events, but only for a single finger
* the Microsoft Surface and other multitouch IE10 devices should deliver pointer events, but I haven't had opportunity to verify my logging code and see it in action myself

You pretty much just load the standalone HTML file in your browser of choice. I tend to use `python -m SimpleHTTPServer 8080` to host this from a [grandpa box](http://dilbert.com/strips/comic/2011-08-03/) to a local network. This repo doubles as an **[online demo](http://natevw.github.com/touch-tester)** — it can be accessed from devices at mobile shops, electronics resellers and nerdly get-togethers!
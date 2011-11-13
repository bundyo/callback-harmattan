Callback/Harmattan
================
Callback/Harmattan is a Qt/QML application library that allows for Callback based projects
to be built for the MeeGo-Harmattan Platform. Callback based applications are, at the core,
an application written with web technology: HTML, CSS and JavaScript.

What works
================

Only the Accelerometer, Geolocation, Notification and Network modules
are working, but we are looking forward to support the other modules as well.

In addition to the regular Callback API there is a Hash module. It allows for calculating 
HMAC-SHA1 hashes (which is too slow to perform in JavaScript on Nokia hardware).

Known Issues
================

When calling navigator.network.isReachable, if the device if not connected, it
will connect to the internet using the default access point *without warning the
user* or letting the user choose what access point to use.

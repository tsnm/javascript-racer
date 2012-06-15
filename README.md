Javascript Pseudo 3D Racer
==========================

How to build an HTML5 Pseudo 3D Racing Game in 4 parts:

 * [Straight Roads](http://codeincomplete.com/experiment/racer/v1.straight.html)
 * [Adding Curves](http://codeincomplete.com/experiment/racer/v2.curves.html)
 * [Adding Hills](http://codeincomplete.com/experiment/racer/v3.hills.html)
 * [Adding Sprites and Collision Detection](http://codeincomplete.com/experiment/racer/v4.final.html)

This is a work-in-progress (June 2012). I plan on writing up 'how to' articles on [codeincomplete.com](http://codeincomplete.com) over the
next week (or two, or three... you know that EURO2012 is on right now, so who knows?).

 * [play the game](http://codeincomplete.com/experiment/racer/v4.final.html)
 * view the [source](https://github.com/jakesgordon/javascript-racer)
 * read about how it works (coming soon)

A note on performance
=====================

The performance of this game is **very** machine/browser dependent. It works quite well in modern
browsers, especially those with GPU canvas acceleration, but a bad graphics driver can kill it stone
dead. So your mileage may vary. There are controls provided to change the rendering resolution
and the draw distance to scale to fit your machine.

Currently supported browsers include:

 * Firefox (v12+) works great, 60fps at high res - Nice!
 * Chrome (v19+) works great, 60fps at high res... provided you dont have a bad GPU driver
 * IE9 - ok, 30fps at medium res... not great, but at least it works

The current state of mobile browser performance is pretty dismal. Dont expect this to be playable on
any mobile device.

>> _NOTE: I havent actually spent anytime optimizing for performance yet. So it might be possible to
   make it play well on older browsers, but that's not really what this project is about._

A note on code structure
========================

This project happens to be implemented in javascript (because its easy for prototyping) but
is not intended to demonstrate javascript techniques or best practices. In fact, in order to
keep it simple to understand it embeds the javascript for each example directly in the HTML
page (horror!) and, even worse, uses global variables and functions (OMG!).

If I was building a real game I would have much more structure and organization to the
code, but since its just a racing game tech demo, I have elected to [KISS](http://en.wikipedia.org/wiki/KISS_principle).

FUTURE
======

It's quite astounding what it takes to actually [finish](http://codeincomplete.com/posts/2011/9/21/defining_finished/)
a game, even a simple one. And this is not a project that I plan on polishing into a finished state. It should
really be considered just how to get started with a psuedo-3d racing game.

If we were to try to turn it into a real game we would have to consider:

 * car sound fx
 * music
 * full screen mode
 * HUD fx (flash on fastest lap, confetti, color coded speedometer, etc)
 * more accurate sprite collision
 * better car AI (steering, braking etc)
 * an actual crash when colliding at high speed
 * more bounce when car is off road
 * screen shake when off-road or collision
 * throw up dirt particles when off road
 * automatic resolution & drawDistance detection
 * projection based curves ? x,y rotation
 * sub-pixel aliasing artifacts on curves
 * smarter fog to cover sprites (blue against sky, cover sprites)
 * multiple stages, different maps
 * a lap map, with current position indicator
 * road splits and joins
 * day/night cycle
 * weather effects
 * tunnels, bridges, clouds, walls, buildings
 * city, desert, ocean
 * add city of seattle and space needle to background
 * 'bad guys' - add some competetor drivers to race against as well as the 'traffic'
 * different game modes - fastest lap, 1-on-1 racing, collect coins ? shoot bad guys ?
 * a whole lot of gameplay tuning
 * ...
 * ...

Related Links
=============

 * http://www.gorenfeld.net/lou/pseudo/
 * http://10k.aneventapart.com/1/Uploads/198/

License
=======

[MIT](http://en.wikipedia.org/wiki/MIT_License) license.


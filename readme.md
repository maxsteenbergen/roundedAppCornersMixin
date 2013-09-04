# Rounded App Corners — SCSS Mixin
A simple, scalable SCSS mixin to give your web app rounded corners against the device's screen edges.

## Live demo
A live demo of the mixin in use can be found [here](http://maxsteenbergen.com/appscargot).

## Usage
The mixin depends on 2 extra elements in your HTML markup. Inside your <code>body</code> tag, preferably just before the closing <code>/body</code> tag, add the following div's:

	<div id="topCorners"></div>
	<div id="bottomCorners"></div>

The mixin takes 1 argument: the size of the radius. Simply add   <code>@include _roundedAppCorners(15px)</code> to your CSS styles for <code>body{}</code>. For bigger or smaller radii, simply replace 15px with any other number. Sticking with px as unit works best.

## Disclaimer
This mixin relies on SVG embedded as Base64 and pseudo-elements. If the browser doesn't support any of these technologies, the mixin will break. It's tested on Mac and iOS only, and works beautifully on those platforms. No guarantees for other platforms.
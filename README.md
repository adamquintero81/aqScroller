## AngularJS Module: 'aqScroller'

Source code for aqScoller, an AngularJS module to facilitate easy-to-implement automatic scrolling to html elements.

## Motivation

I needed a way to simplify automatic scrolling to elements in my AngularJS apps, so I adapted the methods from ngSmoothScroll @ https://github.com/d-oliveros/ngSmoothScroll. All functions, directives, and services are contained within AngularJS , no global namespace used. 

## Code Example

###With the 'aqScroller' module injected as a dependency in your AngularJS app:

* Example scrolls to this element automatically when it is clicked using default settings:<br>
`<div ng-scroller></div>`

* Example scrolls to another element when this element is clicked (element for scroll-to must have an id):<br>
`<div id="element-id"></div>`<br>
`<div ng-scroller scroller-to="{{'element-id'}}"></div>`

* Example scrolls to this element when clicked if(condition = true):<br>
`<div ng-scroller scroller-if="{{'true'}}"></div>`

* Example scrolls to another element when this element is clicked if(condition = true) (element for scroll-to must have an id):<br>
`<div id="element-id"></div>`<br>
`<div ng-scroller scroller-if="{{'true'}}" scroller-to="{{'element-id'}}"></div>`

* Example scrolls using user-defined settings:<br>
`<div ng-scroller scroller-easing="easeInOutQuint" scroller-offset="1" scroller-duration="600"></div>`

## Options

* scroller-to="{{'element-1}}"<br>
--- When this element is clicked, automatically scroll to element with id="element-1"

* scroller-if="{{'true'}}"<br>
--- When this element is clicked, automatically scroll if 'true', do nothing if 'false'.

* scroller-easing="easingFunctionName"<br>
- Valid easing function names:
- Accelerating from zero velocity.
- 'easeInQuad'
- 'easeInCubic'
- 'easeInQuart'
- 'easeInQuint'
- Decelerating to zero velocity.
- 'easeOutQuad'
- 'easeOutCubic'
- 'easeOutQuart'
- 'easeOutQuint'
- Acceleration until halfway, then deceleration.
- 'easeInOutQuad'
- 'easeInOutCubic'
- 'easeInOutQuart'
- 'easeInOutQuint'

* scroller-offset="10"
** Number of pixels to offset the top of scroll to location.

* scroller-duration="600"
** Milliseconds for animation step. Higher numbers give slower animation.

## Installation

Include the script file **after** angular.js in your html:<br>
`<script type="text/javascript" src="angular-ng-scroller.js"></script>`<br>
Inject as a dependency to an AngularJS module.<br>
`angular.module('myApp', ['aqScroller']);`

## License

	AngularJS Module to facilitate smooth scrolling to html elements.
	Copyright (C) 2015  Adam M. Quintero  http://angularadam.com 

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
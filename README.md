## aqScroller AngularJS Module

Source code for aqScoller, an AngularJS module to facilitate easy-to-implement automatic scrolling to html elements.

## Motivation

I needed a way to simplify automatic scrolling to elements in my AngularJS apps, so I adapted the methods from ngSmoothScroll @ https://github.com/d-oliveros/ngSmoothScroll. All functions, directives, and services are contained within AngularJS , no global namespace used. 

## Code Example

###With the 'aqScroller' module injected as a dependency in your AngularJS app:

* Example scrolls to this element automatically when it is clicked using default settings:<br>
`<div ng-scroller></div>`

* Example scrolls to another element when this element is clicked (element for scroll-to must have an id):<br>
`<div id="element-id"></div>`<br>
`<div ng-scroller ng-scroll-to="{{'element-id'}}"></div>`

* Example scrolls to this element when clicked if(condition = true):<br>
`<div ng-scroller ng-scroll-if="{{'true'}}"></div>`

* Example scrolls to another element when this element is clicked if(condition = true) (element for scroll-to must have an id):<br>
`<div id="element-id"></div>`<br>
`<div ng-scroller ng-scroll-if="{{'true'}}" ng-scroll-to="{{'element-id'}}"></div>`

* Example scrolls using user-defined settings:<br>
`<div ng-scroller scroller-easing="easeInOutQuint" scroller-offset="1" scroller-duration="600"></div>`

## Installation

Inject as a dependency to an AngularJS module.

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
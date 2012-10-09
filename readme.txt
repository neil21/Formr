For most explanation and motivation see here:

http://stroadtoboulevard.tumblr.com/formr

The purpose of this webapp is to be able to see the impact of different regulated numbers (setback, height, travel lane and sidewalk width) on the “feel” of the street.

By allowing people to directly manipulate the numbers and see the image change they can see how our current zoning regulations and geometric design guides result in pedestrian-unfriendly car-first streets.

Use cases:

* Easily demonstrate how a block matures over time, from Rural T1 to bustling T5 main street.
* Demonstrate how good enclosure ”feels”.
* Demonstrate how Burnaby’s zoning bylaws and street design guidelines explicitly prevent the development of a Parisian boulevard.
* Show how a multiway boulevard can fit in the same space as a standard Vancouver arterial.
* Show how New Pacific Boulevard will feel (wide street, some trees, no buildings).

With javascript frameworks three.js (webgl - 3D stuff) and dat.gui (controls) this a hell of a lot less difficult than it sounds at first. I’ve done some hacking around, and discovered some quirks of three.js that I’ll happily share. If I could take a week off and hack around I would, but I bet there are young’uns out there that are more time-rich than me.

And I’m sure the urbanism blogosphere would lap it up.

To do:

* general code tidy up: functions, variable names
* presaved settings (dat.gui hopefully makes this easy) with photos for T1 to T6, Vancouver local street, arterial, Paris street, boulevard etc.
* better camera controls (the standard ones messed with dat.gui: maybe just need specific div for rendering to)
* add lots" button
* "vary lot size" slider
* createLane button (and remove lane)
* individual lane widths, heights and colours. (Heights especially important for multi-way boulevards which have a curbed divider between the access lane and the through lanes.)
* some way to choose whether adjustments happen to individual lots, buildings, lanes or to all lots, buildings lanes (see the cubistan example for projecting a ray to select an object - can we select multiple objects? only makes sense to allow multiple select of objects of the same type, i.e. lot, lane or primary building)
* different floor heights
* sloped top floor (roof)
* solid boxes, lighting and shadow (just a question of three.js camera settings)
* add textures
* add trees, cars, people, bikes to street (I'm imagining a single 3D model of each imported from sketchup)
* individual building control - perhaps like cubistan with a selection ray (also include a "select all" button to, e.g., modify all setbacks)
* frill: dynamic measurement brackets showing, for example, lane widths* secondary suites (laneway house, or at least garage)
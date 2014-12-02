# JOSM Workshop

This guide is intended as a primer to becoming a JOSM power user for editing [OpenStreetMap](http://openstreetmap.org). Go [here](https://josm.openstreetmap.de/) to install the latest version of JOSM for your platform of choice.

## Keyboard shortcuts & commands

Command | Name | Description
------- | ---- | -----------
`s`     | Select | Select a feature (tapping it again toggles "lasso" mode)
`x`     | Extrude | Multipurpose tool for creating complex shapes and modifying existing geometry
`q`     | Orthogonalize | Squares up right-angled features, good for property bounds and buildings
`b`     | Building tool | Tool for rapidly tracing buildings _(install [plugin](http://wiki.openstreetmap.org/wiki/JOSM/Plugins/BuildingsTools) for this)_
`m`     | Merge nodes | Helpful for joining two coincident nodes like a park boundary to a coastline
`j`     | Join node to way | Can merge the end of a way to intersect another
`shift-o` | Create circle | Quick tool for making circular features
`g`     | Unglue ways | Disconnects to joined ways from one another
`shift-j` | Join overlapping areas | Merge two overlapping polygons into one (great way to draw complex shapes)
`ctrl-shift-mouse` | Rotate | Rotate selected geometry feature
`f` | Follow tracing | Use when tracing geometry to match another edge, like a `landuse` boundary abutting a coastline
`c` | Combine ways | With two or more joined ways selected, this will merge them into a single way object
`r` | Reverse ways | With a way selected, this will reverse its direction, directionality of ways is only relevant on specific feature types, like one-way streets and waterways (where direction indicates stream flow)
`cmd-c, shift-cmd-v` | Copy & paste tags | A super useful combo when you're adding many independent features with the same or similar tag combination
`a` | Toggle angle snapping | When tracing a way, toggling this will snap your next node to known angles: 30°, 45°, 60°, 90° - helpful for man-made features with geometric shape
`w` | Way improvement mode | Powerful for improvement of existing data. Toggle this on with a way selected and it'll let you reposition nodes along the way, or hold down the `ctrl` key to insert new nodes, making the linework more accurate.
`l` | Align in a line | Align the nodes in a way in a straight line
`tab` | Toggle sidebar | Hide or show the sidebar if you need more editing workspace

## Imagery & data layers

**Bing imagery** is the canonical resource for tracing, usable in most geographies for high resolution base map data.

The **New and Misaligned TIGER Roads** layer is an awesome resource for fixing street data, particularly in areas that don't get much attention. Turning this on will overlay updated TIGER data for newly constructed or changed roadways. This layer is a good tool for adding new roads to the map, and it includes street names. When adding new road geometry or names from this source, you can use the `source=TIGER 2013` tag to attribute new features.

## Presets & tagging

Use the **Presets** menu to browse for tagging presets for common feature types. This is a helpful way to contribute map data with more complex tagging schemas, with many tags that can be difficult to remember, but easy to add.

Tags in OSM can be _very_ complex, and take quite a while to get comfortable with. The [wiki](http://wiki.openstreetmap.org) is the go-to resource for finding out standard tagging methods for different feature types. If you're mapping something obscure and difficult to find on the wiki, you can also use the [OSM help](http://help.openstreetmap.org) Q&A site to ask the community for guidance. The infamous ["map features"](http://wiki.openstreetmap.org/wiki/Map_Features) page is both powerful and daunting.

But remember, most of OpenStreetMap's data standards are by _convention_, so frequency of use for many tag types equals _the correct tagging scheme_. If you're willing to do some digging to find out how to map certain features, [TagInfo](https://taginfo.openstreetmap.org/) is a tool for analyzing the frequency of specific tags to understand what's most widely used globally. Searching for a key like `bridge` shows all the [most commonly used values](https://taginfo.openstreetmap.org/keys/bridge#values).

## GPX Data

If you record [GPS traces](http://wiki.openstreetmap.org/wiki/GPS_Traces) with other applications that publish GPX files, you can drag-and-drop those files into the JOSM workspace to view as reference data for tracing.

## Windows

JOSM has several sidebar windows you can optionally enable depending on what type of mapping you're doing.

### Author

`option-shift-a`

Useful for finding out who last edited a feature. This is a cool way to find out who's mapping in your area, add friends, send messages.

### History

`option-shift-h`

Show full history for a feature (node or way) to see how it's changed over time. Can also link to the changeset in which the feature was last modifed.

### Filter

`option-shift-f`

Extremely useful for minimizing irrelevant clutter on the map. Things like admin boundaries, census data, and landuse can be distracting when you're editing something completely unrelated.

## Plugins

* Building Tools
* Continuous download

## Other features

* **Remote** - allows your JOSM environment to accept remote commands from other applications, like [MapRoulette](http://maproulette.org) or the [Tasking Manager](http://tasks.hotosm.org).
* Data validation
* Custom tile sources
* Look and feel
* Tagging presets
* Add presets to your toolbar

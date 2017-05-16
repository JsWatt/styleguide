# using [D3's amazing wiki](https://github.com/d3/d3/blob/master/API.md) as a starting point

* the point of the below is to figure out how to make my projects more accessible 

* I'll be removing the actual D3 example when I get the chance to actually use this on a project, and then I'll replace with my own code

##structure

* link to readme that has install instructions

* classes/objects/groups

* list of methods/functions that belong to those classes/objects/groups

##start of example from D3

# D3 API Reference

D3 4.0 is a [collection of modules](https://github.com/d3) that are designed to work together; you can use the modules independently, or you can use them together as part of the default build. The source and documentation for each module is available in its repository. Follow the links below to learn more. For changes between 3.x and 4.0, see [CHANGES](https://github.com/d3/d3/blob/master/CHANGES.md); see also the [3.x reference](https://github.com/d3/d3-3.x-api-reference/blob/master/API-Reference.md).

* [Arrays](#arrays-d3-array) ([Statistics](#statistics), [Search](#search), [Transformations](#transformations), [Histograms](#histograms))
* [Axes](#axes-d3-axis)
* [Brushes](#brushes-d3-brush)
* [Chords](#chords-d3-chord)
* [Collections](#collections-d3-collection) ([Objects](#objects), [Maps](#maps), [Sets](#sets), [Nests](#nests))
* [Colors](#colors-d3-color)


D3 uses [semantic versioning](http://semver.org/). The current version is exposed as d3.version.

## [Arrays (d3-array)](https://github.com/d3/d3-array)

Array manipulation, ordering, searching, summarizing, etc.

### [Statistics](https://github.com/d3/d3-array/blob/master/README.md#statistics)

Methods for computing basic summary statistics.

* [d3.min](https://github.com/d3/d3-array/blob/master/README.md#min) - compute the minimum value in an array.
* [d3.max](https://github.com/d3/d3-array/blob/master/README.md#max) - compute the maximum value in an array.
* [d3.extent](https://github.com/d3/d3-array/blob/master/README.md#extent) - compute the minimum and maximum value in an array.
* [d3.sum](https://github.com/d3/d3-array/blob/master/README.md#sum) - compute the sum of an array of numbers.
* [d3.mean](https://github.com/d3/d3-array/blob/master/README.md#mean) - compute the arithmetic mean of an array of numbers.
* [d3.median](https://github.com/d3/d3-array/blob/master/README.md#median) - compute the median of an array of numbers (the 0.5-quantile).
* [d3.quantile](https://github.com/d3/d3-array/blob/master/README.md#quantile) - compute a quantile for a sorted array of numbers.
* [d3.variance](https://github.com/d3/d3-array/blob/master/README.md#variance) - compute the variance of an array of numbers.
* [d3.deviation](https://github.com/d3/d3-array/blob/master/README.md#deviation) - compute the standard deviation of an array of numbers.

### [Search](https://github.com/d3/d3-array/blob/master/README.md#search)

Methods for searching arrays for a specific element.

* [d3.scan](https://github.com/d3/d3-array/blob/master/README.md#scan) - linear search for an element using a comparator.
* [d3.bisect](https://github.com/d3/d3-array/blob/master/README.md#bisect) - binary search for a value in a sorted array.
* [d3.bisectRight](https://github.com/d3/d3-array/blob/master/README.md#bisectRight) - binary search for a value in a sorted array.
* [d3.bisectLeft](https://github.com/d3/d3-array/blob/master/README.md#bisectLeft) - binary search for a value in a sorted array.
* [d3.bisector](https://github.com/d3/d3-array/blob/master/README.md#bisector) - bisect using an accessor or comparator.
* [*bisector*.left](https://github.com/d3/d3-array/blob/master/README.md#bisector_left) - bisectLeft, with the given comparator.
* [*bisector*.right](https://github.com/d3/d3-array/blob/master/README.md#bisector_right) - bisectRight, with the given comparator.
* [d3.ascending](https://github.com/d3/d3-array/blob/master/README.md#ascending) - compute the natural order of two values.
* [d3.descending](https://github.com/d3/d3-array/blob/master/README.md#descending) - compute the natural order of two values.

### [Transformations](https://github.com/d3/d3-array/blob/master/README.md#transformations)

Methods for transforming arrays and for generating new arrays.

* [d3.cross](https://github.com/d3/d3-array/blob/master/README.md#cross) - compute the Cartesian product of two arrays.
* [d3.merge](https://github.com/d3/d3-array/blob/master/README.md#merge) - merge multiple arrays into one array.
* [d3.pairs](https://github.com/d3/d3-array/blob/master/README.md#pairs) - create an array of adjacent pairs of elements.
* [d3.permute](https://github.com/d3/d3-array/blob/master/README.md#permute) - reorder an array of elements according to an array of indexes.
* [d3.shuffle](https://github.com/d3/d3-array/blob/master/README.md#shuffle) - randomize the order of an array.
* [d3.ticks](https://github.com/d3/d3-array/blob/master/README.md#ticks) - generate representative values from a numeric interval.
* [d3.tickIncrement](https://github.com/d3/d3-array/blob/master/README.md#tickIncrement) - generate representative values from a numeric interval.
* [d3.tickStep](https://github.com/d3/d3-array/blob/master/README.md#tickStep) - generate representative values from a numeric interval.
* [d3.range](https://github.com/d3/d3-array/blob/master/README.md#range) - generate a range of numeric values.
* [d3.transpose](https://github.com/d3/d3-array/blob/master/README.md#transpose) - transpose an array of arrays.
* [d3.zip](https://github.com/d3/d3-array/blob/master/README.md#zip) - transpose a variable number of arrays.

### [Histograms](https://github.com/d3/d3-array/blob/master/README.md#histograms)

Bin discrete samples into continuous, non-overlapping intervals.

* [d3.histogram](https://github.com/d3/d3-array/blob/master/README.md#histogram) - create a new histogram generator.
* [*histogram*](https://github.com/d3/d3-array/blob/master/README.md#_histogram) - compute the histogram for the given array of samples.
* [*histogram*.value](https://github.com/d3/d3-array/blob/master/README.md#histogram_value) - specify a value accessor for each sample.
* [*histogram*.domain](https://github.com/d3/d3-array/blob/master/README.md#histogram_domain) - specify the interval of observable values.
* [*histogram*.thresholds](https://github.com/d3/d3-array/blob/master/README.md#histogram_thresholds) - specify how values are divided into bins.
* [d3.thresholdFreedmanDiaconis](https://github.com/d3/d3-array/blob/master/README.md#thresholdFreedmanDiaconis) - the Freedman–Diaconis binning rule.
* [d3.thresholdScott](https://github.com/d3/d3-array/blob/master/README.md#thresholdScott) - Scott’s normal reference binning rule.
* [d3.thresholdSturges](https://github.com/d3/d3-array/blob/master/README.md#thresholdSturges) - Sturges’ binning formula.

## [Axes (d3-axis)](https://github.com/d3/d3-axis)

Human-readable reference marks for scales.

* [d3.axisTop](https://github.com/d3/d3-axis/blob/master/README.md#axisTop) - create a new top-oriented axis generator.
* [d3.axisRight](https://github.com/d3/d3-axis/blob/master/README.md#axisRight) - create a new right-oriented axis generator.
* [d3.axisBottom](https://github.com/d3/d3-axis/blob/master/README.md#axisBottom) - create a new bottom-oriented axis generator.
* [d3.axisLeft](https://github.com/d3/d3-axis/blob/master/README.md#axisLeft) - create a new left-oriented axis generator.
* [*axis*](https://github.com/d3/d3-axis/blob/master/README.md#_axis) - generate an axis for the given selection.
* [*axis*.scale](https://github.com/d3/d3-axis/blob/master/README.md#axis_scale) - set the scale.
* [*axis*.ticks](https://github.com/d3/d3-axis/blob/master/README.md#axis_ticks) - customize how ticks are generated and formatted.
* [*axis*.tickArguments](https://github.com/d3/d3-axis/blob/master/README.md#axis_tickArguments) - customize how ticks are generated and formatted.
* [*axis*.tickValues](https://github.com/d3/d3-axis/blob/master/README.md#axis_tickValues) - set the tick values explicitly.
* [*axis*.tickFormat](https://github.com/d3/d3-axis/blob/master/README.md#axis_tickFormat) - set the tick format explicitly.
* [*axis*.tickSize](https://github.com/d3/d3-axis/blob/master/README.md#axis_tickSize) - set the size of the ticks.
* [*axis*.tickSizeInner](https://github.com/d3/d3-axis/blob/master/README.md#axis_tickSizeInner) - set the size of inner ticks.
* [*axis*.tickSizeOuter](https://github.com/d3/d3-axis/blob/master/README.md#axis_tickSizeOuter) - set the size of outer (extent) ticks.
* [*axis*.tickPadding](https://github.com/d3/d3-axis/blob/master/README.md#axis_tickPadding) - set the padding between ticks and labels.

## [Brushes (d3-brush)](https://github.com/d3/d3-brush)

Select a one- or two-dimensional region using the mouse or touch.

* [d3.brush](https://github.com/d3/d3-brush/blob/master/README.md#brush) - create a new two-dimensional brush.
* [d3.brushX](https://github.com/d3/d3-brush/blob/master/README.md#brushX) - create a brush along the *x*-dimension.
* [d3.brushY](https://github.com/d3/d3-brush/blob/master/README.md#brushY) - create a brush along the *y*-dimension.
* [*brush*](https://github.com/d3/d3-brush/blob/master/README.md#_brush) - apply the brush to a selection.
* [*brush*.move](https://github.com/d3/d3-brush/blob/master/README.md#brush_move) - move the brush selection.
* [*brush*.extent](https://github.com/d3/d3-brush/blob/master/README.md#brush_extent) - define the brushable region.
* [*brush*.filter](https://github.com/d3/d3-brush/blob/master/README.md#brush_filter) - control which input events initiate brushing.
* [*brush*.handleSize](https://github.com/d3/d3-brush/blob/master/README.md#brush_handleSize) - set the size of the brush handles.
* [*brush*.on](https://github.com/d3/d3-brush/blob/master/README.md#brush_on) - listen for brush events.
* [d3.brushSelection](https://github.com/d3/d3-brush/blob/master/README.md#brushSelection) - get the brush selection for a given node.

## [Chords (d3-chord)](https://github.com/d3/d3-chord)

* [d3.chord](https://github.com/d3/d3-chord/blob/master/README.md#chord) - create a new chord layout.
* [*chord*](https://github.com/d3/d3-chord/blob/master/README.md#_chord) - compute the layout for the given matrix.
* [*chord*.padAngle](https://github.com/d3/d3-chord/blob/master/README.md#chord_padAngle) - set the padding between adjacent groups.
* [*chord*.sortGroups](https://github.com/d3/d3-chord/blob/master/README.md#chord_sortGroups) - define the group order.
* [*chord*.sortSubgroups](https://github.com/d3/d3-chord/blob/master/README.md#chord_sortSubgroups) - define the source and target order within groups.
* [*chord*.sortChords](https://github.com/d3/d3-chord/blob/master/README.md#chord_sortChords) - define the chord order across groups.
* [d3.ribbon](https://github.com/d3/d3-chord/blob/master/README.md#ribbon) - create a ribbon shape generator.
* [*ribbon*](https://github.com/d3/d3-chord/blob/master/README.md#_ribbon) - generate a ribbon shape.
* [*ribbon*.source](https://github.com/d3/d3-chord/blob/master/README.md#ribbon_source) - set the source accessor.
* [*ribbon*.target](https://github.com/d3/d3-chord/blob/master/README.md#ribbon_target) - set the target accessor.
* [*ribbon*.radius](https://github.com/d3/d3-chord/blob/master/README.md#ribbon_radius) - set the ribbon source or target radius.
* [*ribbon*.startAngle](https://github.com/d3/d3-chord/blob/master/README.md#ribbon_startAngle) - set the ribbon source or target start angle.
* [*ribbon*.endAngle](https://github.com/d3/d3-chord/blob/master/README.md#ribbon_endAngle) - set the ribbon source or target end angle.
* [*ribbon*.context](https://github.com/d3/d3-chord/blob/master/README.md#ribbon_context) - set the render context.

## [Collections (d3-collection)](https://github.com/d3/d3-collection)

Handy data structures for elements keyed by string.

### [Objects](https://github.com/d3/d3-collection/blob/master/README.md#objects)

Methods for converting associative arrays (objects) to arrays.

* [d3.keys](https://github.com/d3/d3-collection/blob/master/README.md#keys) - list the keys of an associative array.
* [d3.values](https://github.com/d3/d3-collection/blob/master/README.md#values) - list the values of an associated array.
* [d3.entries](https://github.com/d3/d3-collection/blob/master/README.md#entries) - list the key-value entries of an associative array.

### [Maps](https://github.com/d3/d3-collection/blob/master/README.md#maps)

Like ES6 Map, but with string keys and a few other differences.

* [d3.map](https://github.com/d3/d3-collection/blob/master/README.md#map) - create a new, empty map.
* [*map*.has](https://github.com/d3/d3-collection/blob/master/README.md#map_has) - returns true if the map contains the given key.
* [*map*.get](https://github.com/d3/d3-collection/blob/master/README.md#map_get) - get the value for the given key.
* [*map*.set](https://github.com/d3/d3-collection/blob/master/README.md#map_set) - set the value for the given key.
* [*map*.remove](https://github.com/d3/d3-collection/blob/master/README.md#map_remove) - remove the entry for given key.
* [*map*.clear](https://github.com/d3/d3-collection/blob/master/README.md#map_clear) - remove all entries.
* [*map*.keys](https://github.com/d3/d3-collection/blob/master/README.md#map_keys) - get the array of keys.
* [*map*.values](https://github.com/d3/d3-collection/blob/master/README.md#map_values) - get the array of values.
* [*map*.entries](https://github.com/d3/d3-collection/blob/master/README.md#map_entries) - get the array of entries (key-values objects).
* [*map*.each](https://github.com/d3/d3-collection/blob/master/README.md#map_each) - call a function for each entry.
* [*map*.empty](https://github.com/d3/d3-collection/blob/master/README.md#map_empty) - returns false if the map has at least one entry.
* [*map*.size](https://github.com/d3/d3-collection/blob/master/README.md#map_size) - compute the number of entries.

### [Sets](https://github.com/d3/d3-collection/blob/master/README.md#sets)

Like ES6 Set, but with string keys and a few other differences.

* [d3.set](https://github.com/d3/d3-collection/blob/master/README.md#set) - create a new, empty set.
* [*set*.has](https://github.com/d3/d3-collection/blob/master/README.md#set_has) - returns true if the set contains the given value.
* [*set*.add](https://github.com/d3/d3-collection/blob/master/README.md#set_add) - add the given value.
* [*set*.remove](https://github.com/d3/d3-collection/blob/master/README.md#set_remove) - remove the given value.
* [*set*.clear](https://github.com/d3/d3-collection/blob/master/README.md#set_clear) - remove all values.
* [*set*.values](https://github.com/d3/d3-collection/blob/master/README.md#set_values) - get the array of values.
* [*set*.each](https://github.com/d3/d3-collection/blob/master/README.md#set_each) - call a function for each value.
* [*set*.empty](https://github.com/d3/d3-collection/blob/master/README.md#set_empty) - returns true if the set has at least one value.
* [*set*.size](https://github.com/d3/d3-collection/blob/master/README.md#set_size) - compute the number of values.

### [Nests](https://github.com/d3/d3-collection/blob/master/README.md#nests)

Group data into arbitrary hierarchies.

* [d3.nest](https://github.com/d3/d3-collection/blob/master/README.md#nest) - create a new nest generator.
* [*nest*.key](https://github.com/d3/d3-collection/blob/master/README.md#nest_key) - add a level to the nest hierarchy.
* [*nest*.sortKeys](https://github.com/d3/d3-collection/blob/master/README.md#nest_sortKeys) - sort the current nest level by key.
* [*nest*.sortValues](https://github.com/d3/d3-collection/blob/master/README.md#nest_sortValues) - sort the leaf nest level by value.
* [*nest*.rollup](https://github.com/d3/d3-collection/blob/master/README.md#nest_rollup) - specify a rollup function for leaf values.
* [*nest*.map](https://github.com/d3/d3-collection/blob/master/README.md#nest_map) - generate the nest, returning a map.
* [*nest*.object](https://github.com/d3/d3-collection/blob/master/README.md#nest_object) - generate the nest, returning an associative array.
* [*nest*.entries](https://github.com/d3/d3-collection/blob/master/README.md#nest_entries) - generate the nest, returning an array of key-values tuples.

## [Colors (d3-color)](https://github.com/d3/d3-color)

Color manipulation and color space conversion.

* [d3.color](https://github.com/d3/d3-color/blob/master/README.md#color) - parse the given CSS color specifier.
* [*color*.rgb](https://github.com/d3/d3-color/blob/master/README.md#color_rgb) - compute the RGB equivalent of this color.
* [*color*.brighter](https://github.com/d3/d3-color/blob/master/README.md#color_brighter) - create a brighter copy of this color.
* [*color*.darker](https://github.com/d3/d3-color/blob/master/README.md#color_darker) - create a darker copy of this color.
* [*color*.displayable](https://github.com/d3/d3-color/blob/master/README.md#color_displayable) - returns true if the color is displayable on standard hardware.
* [*color*.toString](https://github.com/d3/d3-color/blob/master/README.md#color_toString) - format the color as an RGB hexadecimal string.
* [d3.rgb](https://github.com/d3/d3-color/blob/master/README.md#rgb) - create a new RGB color.
* [d3.hsl](https://github.com/d3/d3-color/blob/master/README.md#hsl) - create a new HSL color.
* [d3.lab](https://github.com/d3/d3-color/blob/master/README.md#lab) - create a new Lab color.
* [d3.hcl](https://github.com/d3/d3-color/blob/master/README.md#hcl) - create a new HCL color.
* [d3.cubehelix](https://github.com/d3/d3-color/blob/master/README.md#cubehelix) - create a new Cubehelix color.

# Milo CSS Utilities
An array of CSS Utility classes to be used in your Milo CSS-based framework.

## Installation
```npm i @milo-css/utilities```

## Utilities
### Clearfix
```@import "node_modules/@milo-css/utilities/clearfix";```

| Class | Description | Note |
|---|---|---|
| ```clearfix``` | Clear a floating element | Requires ```@milo-css/mixins/clearfix``` |


### Color
```@import "node_modules/@milo-css/utilities/color";```

Utility classes for ```background-color``` and ```color``` are created from the colours defined within a ```colors()``` map variable. Additional utility classes will be added by adding more key-value pairs to this map.

The variables below are provided by default but can be merged with or overridden in your framework:

```Shell
$colors: () !default;
$colors: map-merge(
    (
        // Required base colours
        "white":                rgb(255, 255, 255),
        "black":                rgb(17, 17, 17),
        "primary":              rgb(10, 211, 255),
        "secondary":            rgb(235, 236, 238)
    ),
    $colors
);
```

The variables above will compile to generate the following classes:

| Class | Description |
|---|---|
| ```b-white``` | Sets the background color to white |
| ```b-black``` | Sets the background color to black |
| ```b-primary``` | Sets the background color to primary |
| ```b-secondary``` | Sets the background color to secondary |
| ```c-white``` | Sets the text color to white |
| ```c-black``` | Sets the text color to black |
| ```c-primary``` | Sets the text color to primary |
| ```c-secondary``` | Sets the text color to secondary |


### Display
```@import "node_modules/@milo-css/utilities/display";```

| Class | Description |
|---|---|
| ```d-block``` | Display as a block element |
| ```d-hidden``` | Display as a hidden element |
| ```d-flex``` | Display as a fles element |
| ```d-grid``` | Display as a grid element |
| ```d-inline```  | Display as a inline element |
| ```d-inline-block``` | Display as a inline block element |
| ```d-inline-flex``` | Display as a inline flex element |
| ```d-table``` | Display as a table element |
| ```d-table-cell``` | Display as a table cell element |


### Flex
```@import "node_modules/@milo-css/utilities/flex";```

Use all the below with ```d-flex``` on the container of the items to be flexed.

A good resource on flex can be found at [css-tricks.com](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).

| Class | Description |
|---|---|
| _**Directions**_||
| ```flex-row``` | Sets the direction to row |
| ```flex-column``` | Sets the direction to column |
| ```flex-row-reverse``` | Sets the direction to row reverse |
| ```flex-column-reverse``` | Sets the direction to row column |
| _**Wrap**_ ||
| ```flex-nowrap``` | Single-line which may cause the container to overflow |
| ```flex-wrap``` | Multi-lines, direction is defined by ```flex-direction``` |
| ```flex-wrap-reverse``` | Multi-lines, opposite to direction defined by ```flex-direction``` |
| _**Justify Content** - defines the alignment along the main axis_ ||
| ```justify-content-start``` | Justify child items on main axis to ```flex-start``` |
| ```justify-content-end``` | Justify child items on main axis to ```flex-end``` |
| ```justify-content-center``` | Justify child items on main axis to ```center``` |
| ```justify-content-between``` | Justify child items on main axis to ```space-between``` |
| ```justify-content-around``` | Justify child items on main axis to ```space-around``` |
| ```justify-content-evenly``` | Justify child items on main axis to ```space-evenly``` |
| _**Align Items** - defines the alignment along the cross axis on the current line_ ||
| ```align-items-start``` |	Align child items on cross axis to ```flex-start``` |
| ```align-items-end``` | Align child items on cross axis to ```flex-end``` |
| ```align-items-center``` | Align child items on cross axis to ```center``` |
| ```align-items-baseline``` | Align child items on cross axis to ```baseline``` |
| ```align-items-stretch``` | Align child items on cross axis to ```stretch``` |
| _**Align Content** - aligns lines within a flex container when there is extra space in the cross-axis_ ||
| ```align-content-start``` | Align content on cross axis to ```flex-start``` |
| ```align-content-end``` | Align content on cross axis to ```flex-end``` |
| ```align-content-center``` | Align content on cross axis to ```center``` |
| ```align-content-between``` | Align content on cross axis to ```space-between``` |
| ```align-content-around``` | Align content on cross axis to ```space-around``` |
| ```align-content-stretch``` | Align content on cross axis to ```stretch``` |
| _**Align Self** - override default alignment (or the one specified by_ ```align-items```_) for individual flex items_ ||
| ```align-self-start``` | Align item on cross axis to ```flex-start``` |
| ```align-self-end``` | Align item on cross axis to ```flex-end``` |
| ```align-self-center``` | Align item on cross axis to ```center``` |
| ```align-self-baseline``` | Align item on cross axis to ```baseline``` |
| ```align-self-stretch``` | Align item on cross axis to ```stretch``` |


### Float
```@import "node_modules/@milo-css/utilities/float";```

| Class | Description |
|---|---|
| ```pull-left``` | Float an element to the left |
| ```pull-right``` | Float an element to the right |


### Grid
```@import "node_modules/@milo-css/utilities/grid";```

Use all the below with ```d-grid``` position all grid items wihin the parent container.

A good resource on flex can be found at [css-tricks.com](https://css-tricks.com/snippets/css/complete-guide-grid/).

| Class | Description |
|---|---|
| _**Justify Items** - defines the alignment of grid items along the inline (row) axis_ ||
| ```grid-justify-items-start``` | Justify grid items flush with the start edge of their cell |
| ```grid-justify-items-end``` | Justify grid items flush with the end edge of their cell |
| ```grid-justify-items-center``` | Justify grid items with the center of their cell |
| ```grid-justify-items-stretch``` | Set grid items to fill the whole width of their cell |
| _**Align Items** - defines the alignment of grid items along the block (column) axis_ ||
| ```grid-align-items-start``` | Align grid items flush with the start edge of their cell |
| ```grid-align-items-end``` | Align grid items flush with the end edge of their cell |
| ```grid-align-items-center``` | Align grid items with the center of their cell |
| ```grid-align-items-stretch``` | Set grid items to fill the whole height of their cell |
| _**Justify Content** - defines the alignment of the grid along the inline (row) axis_ ||
| ```grid-justify-content-start``` | Aligns the grid to be flush with the start edge of the grid container |
| ```grid-justify-content-end``` | Aligns the grid to be flush with the end edge of the grid container |
| ```grid-justify-content-center``` | Aligns the grid in the center of the grid container |
| ```grid-justify-content-stretch``` | Resizes the grid items to allow the grid to fill the full width of the grid container |
| ```grid-justify-content-between``` | Places an even amount of space between each grid item, with no space at the far ends |
| ```grid-justify-content-around``` | Places an even amount of space between each grid item, with half-sized spaces on the far ends |
| ```grid-justify-content-evenly``` | Places an even amount of space between each grid item, including the far ends |
| _**Align Content** - defines the alignment of the grid along the block (column) axis_ ||
| ```grid-align-content-start``` | Aligns the grid to be flush with the start edge of the grid container |
| ```grid-align-content-end``` | Aligns the grid to be flush with the end edge of the grid container |
| ```grid-align-content-center``` | Aligns the grid in the center of the grid container |
| ```grid-align-content-stretch``` | Resizes the grid items to allow the grid to fill the full height of the grid container |
| ```grid-align-content-between``` | Places an even amount of space between each grid item, with no space at the far ends |
| ```grid-align-content-around``` | Places an even amount of space between each grid item, with half-sized spaces on the far ends |
| ```grid-align-content-evenly``` | Places an even amount of space between each grid item, including the far ends |


### Image
```@import "node_modules/@milo-css/utilities/image";```

| Class | Description | Note |
|---|---|---|
| ```img-fluid``` | Make an image responsive and use the full width but no more | Requires ```@milo-css/mixins/img-fluid``` |


### List
```@import "node_modules/@milo-css/utilities/list";```

Utility classes to be applied to a ```<ul>``` or ```<ol>``` element. The variable below are provided by default but can be overridden in your framework:

```Shell
$list-inline-elem-margin-x:     1rem !default;
```

| Class | Description |
|---|---|
| ```list-style-none``` | Remove bullets from a ```<ul>``` or ```<ol>``` element |
| ```list-style-reset``` | Remove list style, padding and margin from a ```<ul>``` or ```<ol>``` element |
| ```list-inline``` | Resets list style of a ```<ul>``` or ```<ol>``` element and displays its children inline |


### Overflow
```@import "node_modules/@milo-css/utilities/overflow";```

| Class | Description |
|---|---|
| ```noscroll``` | Sets overflow to hidden |
| ```scroll-x``` | Allow scrolling horizontally when required |


### Position
```@import "node_modules/@milo-css/utilities/position";```

| Class | Description |
|---|---|
| ```relative``` | Sets position to relative |
| ```absolute``` | Sets position to absolute |
| ```fixed``` | Sets position to fixed |
| ```sticky``` | Sets position to sticky |


### Sizing
```@import "node_modules/@milo-css/utilities/sizing";```

| Class | Description |
|---|---|
| ```full-height``` | Sets the height to 100% |
| ```full-viewport-height``` | Sets the height to 100% of the viewport height |
| ```full-width``` | Sets the width to 100% |
| ```full-max-width``` | Sets the max width to 100% |


### Spacing
```@import "node_modules/@milo-css/utilities/spacing";```

Produces semantic classes for all margin & padding properties based on a base value applied to keys defined within a ```spacers()``` map variable. 

The variables below are provided by default but can be overridden in your framework:

```Shell
$base-spacer:               1rem !default;
$base-spacer-y:             $base-spacer !default;
$base-spacer-x:             $base-spacer !default;

$spacers: (
    // Size     // Lengths
    "0":        (x: 0, y: 0),
    "h":        (x: ($base-spacer-x * .5), y: ($base-spacer-y * .5)),
    "1":        (x: $base-spacer-x, y: $base-spacer-y),
    "1h":       (x: ($base-spacer-x * 1.5), y: ($base-spacer-y * 1.5)),
    "2":        (x: ($base-spacer-x * 2), y: ($base-spacer-y * 2)),
    "2h":       (x: ($base-spacer-x * 2.5), y: ($base-spacer-y * 2.5)),
    "3":        (x: ($base-spacer-x * 3), y: ($base-spacer-y * 3)),
    "4":        (x: ($base-spacer-x * 4), y: ($base-spacer-y * 4)),
    "5":        (x: ($base-spacer-x * 5), y: ($base-spacer-y * 5)),
    "6":        (x: ($base-spacer-x * 6), y: ($base-spacer-y * 6)),
    "7":        (x: ($base-spacer-x * 7), y: ($base-spacer-y * 7)),
    "8":        (x: ($base-spacer-x * 8), y: ($base-spacer-y * 8)),
    "9":        (x: ($base-spacer-x * 9), y: ($base-spacer-y * 9)),
    "10":       (x: ($base-spacer-x * 10), y: ($base-spacer-y * 10)),
) !default;
```

The variables above will compile to generate the following classes for each variable outlined in the ```spacers()``` map where ```XX``` is the key, eg. ```mt-1h```:

| Class | Description |
|---|---|
| _**Margin**_ ||
| ```m-XX``` | Sets margin on all sides |
| ```mt-XX``` | Sets ```margin-top``` |
| ```mr-XX``` | Sets ```margin-right``` |
| ```mb-XX``` | Sets ```margin-bottom``` |
| ```ml-XX``` | Sets ```margin-left``` |
| ```mx-XX``` | Sets a margin on the x (horizontal) axis |
| ```my-XX``` | Sets a margin on the y (vertical) axis |
| _**Padding**_ ||
| ```p-XX``` | Sets padding on all sides |
| ```pt-XX``` | Sets ```padding-top``` |
| ```pr-XX``` | Sets ```padding-right``` |
| ```pb-XX``` | Sets ```padding-bottom``` |
| ```pl-XX``` | Sets ```padding-left``` |
| ```px-XX``` | Sets a padding on the x (horizontal) axis |
| ```py-XX``` | Sets a padding on the y (vertical) axis |

The following classes are also included:

| Class | Description | Note |
|---|---|---|
| _**Margin**_ ||
| ```margin-zero``` | Sets margin on all side to zero ||
| ```m-auto``` | Sets margin on all side to ```auto``` ||
| ```mt-auto``` | Sets ```margin-top``` to ```auto``` ||
| ```mr-auto``` | Sets ```margin-right``` to ```auto``` ||
| ```mb-auto``` | Sets ```margin-bottom``` to ```auto``` ||
| ```ml-auto``` | Sets ```margin-left``` to ```auto``` ||
| _**Padding**_ ||
| ```padding-zero``` | Sets padding on all side to zero ||
| _**Push**_ ||
| ```push-auto``` | Sets margin on the x (horizontal) axis to ```auto``` | Requires ```@milo-css/mixins/push-auto``` |


### Text
```@import "node_modules/@milo-css/utilities/text";```

Utility classes to be applied to text-based elements. The variables below are provided by default but can be overridden in your framework:

```Shell
$strong-font-weight:        700 !default;
$lead-font-weight:          600 !default;
$small-font-size:           80% !default;
$muted-opacity:             .6 !default;
```

| Class | Description |
|---|---|
| _**Text Align**_ ||
| ```text-left``` | Sets text alignment to left |
| ```text-right``` | Sets text alignment to right |
| ```text-center``` | Sets text alignment to center |
| ```text-justify``` | Sets text alignment to justify |
| _**Other**_ ||
| ```strong``` | Sets font weight to strong |
| ```lead``` | Sets font weight to value of ```$lead-font-weight``` |
| ```muted``` | Sets the opacity to muted |
| ```nowrap``` | Stops the text from wrapping |
| ```small``` | Sets font size to small |
| ```uppercase``` | Makes the text uppercase |


### Visibility
```@import "node_modules/@milo-css/utilities/visibility";```

Utility classes for ```background-color``` and ```color``` are created from the colours defined within a ```colors()``` map variable. Additional utility classes will be added by adding more key-value pairs to this map.

Produces semantic classes for hiding element based on values defined within a ```viewport-breakpoints()``` map variable. 

The variables below are provided by default but can be overridden in your framework:

```Shell
$viewport-breakpoints: (
    xs: 0,
    sm: 576px,
    md: 768px,
    lg: 992px,
    xl: 1200px
) !default;
```

The variables above will compile to generate the following classes:

| Class | Description | Note |
|---|---|---|
| ```hidden-xs``` | Hide this element on the xs breakpoint only | Requires ```media-breakpoint-only()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-sm``` | Hide this element on the sm breakpoint only | Requires ```media-breakpoint-only()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-md``` | Hide this element on the md breakpoint only | Requires ```media-breakpoint-only()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-lg``` | Hide this element on the lg breakpoint only | Requires ```media-breakpoint-only()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-xl``` | Hide this element on the xl breakpoint only | Requires ```media-breakpoint-only()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-xs-down``` | Hide this element on the xs breakpoint and lower | Requires ```media-breakpoint-down()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-sm-down``` | Hide this element on the sm breakpoint and lower | Requires ```media-breakpoint-down()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-md-down``` | Hide this element on the md breakpoint and lower | Requires ```media-breakpoint-down()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-lg-down``` | Hide this element on the lg breakpoint and lower | Requires ```media-breakpoint-down()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-xl-down``` | Hide this element on the xl breakpoint and lower | Requires ```media-breakpoint-down()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-xs-up``` | Hide this element on the xs breakpoint and higher | Requires ```media-breakpoint-up()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-sm-up``` | Hide this element on the sm breakpoint and higher | Requires ```media-breakpoint-up()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-md-up``` | Hide this element on the md breakpoint and higher | Requires ```media-breakpoint-up()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-lg-up``` | Hide this element on the lg breakpoint and higher | Requires ```media-breakpoint-up()``` mixin thats part of ```@milo-css/grid``` module |
| ```hidden-xl-up``` | Hide this element on the xl breakpoint and higher | Requires ```media-breakpoint-up()``` mixin thats part of ```@milo-css/grid``` module |

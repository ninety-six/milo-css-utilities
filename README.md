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

The below are provided by default but can be merged with or overridden in your framework:
- ```white``` (#FFFFFF, rgb(255, 255, 255))
- ```black``` (#111111, rgb(17, 17, 17))
- ```primary``` (#0AD3FF, rgb(10, 211, 255))
- ```secondary``` (#EBECEE, rgb(235, 236, 238))

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
| *Directions* ||
| ```flex-row``` | Sets the direction to row |
| ```flex-column``` | Sets the direction to column |
| ```flex-row-reverse``` | Sets the direction to row reverse |
| ```flex-column-reverse``` | Sets the direction to row column |
| *Wrap* ||
| ```flex-nowrap``` | Single-line which may cause the container to overflow |
| ```flex-wrap``` | Multi-lines, direction is defined by ```flex-direction``` |
| ```flex-wrap-reverse``` | Multi-lines, opposite to direction defined by ```flex-direction``` |
| *Justify Content - defines the alignment along the main axis* ||
| ```justify-content-start``` | Justify child items on main axis to ```flex-start``` |
| ```justify-content-end``` | Justify child items on main axis to ```flex-end``` |
| ```justify-content-center``` | Justify child items on main axis to ```center``` |
| ```justify-content-between``` | Justify child items on main axis to ```space-between``` |
| ```justify-content-around``` | Justify child items on main axis to ```space-around``` |
| ```justify-content-evenly``` | Justify child items on main axis to ```space-evenly``` |
| *Align Items - defines the alignment along the cross axis on the current line* ||
| ```align-items-start``` |	Align child items on cross axis to ```flex-start``` |
| ```align-items-end``` | Align child items on cross axis to ```flex-end``` |
| ```align-items-center``` | Align child items on cross axis to ```center``` |
| ```align-items-baseline``` | Align child items on cross axis to ```baseline``` |
| ```align-items-stretch``` | Align child items on cross axis to ```stretch``` |
| *Align Content - aligns lines within a flex container when there is extra space in the cross-axis* ||
| ```align-content-start``` | Align content on cross axis to ```flex-start``` |
| ```align-content-end``` | Align content on cross axis to ```flex-end``` |
| ```align-content-center``` | Align content on cross axis to ```center``` |
| ```align-content-between``` | Align content on cross axis to ```space-between``` |
| ```align-content-around``` | Align content on cross axis to ```space-around``` |
| ```align-content-stretch``` | Align content on cross axis to ```stretch``` |
| *Align Self - override default alignment (or the one specified by ```align-items```) for individual flex items* ||
| ```align-self-start``` | Align item on cross axis to ```flex-start``` |
| ```align-self-end``` | Align item on cross axis to ```flex-end``` |
| ```align-self-center``` | Align item on cross axis to ```center``` |
| ```align-self-baseline``` | Align item on cross axis to ```baseline``` |
| ```align-self-stretch``` | Align item on cross axis to ```stretch``` |



### Spacing
```@import "node_modules/@milo-css/utilities/spacing";```

Produces semantic classes for all margin & padding properties based on a base value.
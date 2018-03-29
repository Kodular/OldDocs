# Vertical Arrangement

Use a vertical arrangement component to display a group of components laid out from top to bottom, left-aligned.

This component is a formatting element in which you place components that should be displayed one below another. The first child component is stored on top, the second beneath it, and so on. If you want to have components displayed next to one another, use HorizontalArrangement instead.

In a VerticalArrangement, components are arranged along the vertical axis, left-aligned.

If a VerticalArrangement's Width property is set to Automatic, the actual width of the arrangement is determined by the widest component in the arrangement whose Width property is not set to Fill Parent. If a VerticalArrangement's Width property is set to Automatic and it contains only components whose Width properties are set to Fill Parent, the actual width of the arrangement is calculated using the automatic widths of the components. If a VerticalArrangement's Width property is set to Automatic and it is empty, the width will be 100.

If a VerticalArrangement's Height property is set to Automatic, the actual height of the arrangement is determined by the sum of the heights of the components. If a VerticalArrangement's Height property is set to Automatic, any components whose Height properties are set to Fill Parent will behave as if they were set to Automatic.

If a VerticalArrangement's Height property is set to Fill Parent or specified in pixels, any components whose Height properties are set to Fill Parent will equally take up the height not occupied by other components.

## Properties

### AlignHorizontal

A number that encodes how contents of the arrangement are aligned horizontally. The choices are: 1 = left aligned, 2 = horizontally centered, 3 = right aligned. Alignment has no effect if the arrangement's width is automatic.

### AlignVertical

A number that encodes how the contents of the arrangement are aligned vertically. The choices are: 1 = aligned at the top, 2 = vertically centered, 3 = aligned at the bottom. Alignment has no effect if the arrangement's height is automatic.

### BackgroundColor

Background color for this component

### Image

Background image for this component

### Visible

If true, component and its contents are visible.

### Height

Vertical arrangement height \(y-size\).

### Width

Vertical arrangement width \(x-size\).


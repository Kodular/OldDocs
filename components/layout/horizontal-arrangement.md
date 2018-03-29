# Horizontal Arrangement

Use a horizontal arrangement component to display a group of components laid out from left to right.

This component is a formatting element in which you place components that should be displayed from left to right. If you want to have components displayed one over another, use VerticalArrangement instead.

In a HorizontalArrangement, components are arranged along the horizontal axis, vertically center-aligned.

If a HorizontalArrangement's Height property is set to Automatic, the actual height of the arrangement is determined by the tallest component in the arrangement whose Height property is not set to Fill Parent. If a HorizontalArrangment's Height property is set to Automatic and it contains only components whose Height properties are set to Fill Parent, the actual height of the arrangement is calculated using the automatic heights of the components. If a HorizontalArrangement's Height property is set to Automatic and it is empty, the height will be 100.

If a HorizontalArrangement's Width property is set to Automatic, the actual width of the arrangement is determined by the sum of the widths of the components. If a HorizontalArrangement's Width property is set to Automatic, any components whose Width properties are set to Fill Parent will behave as if they were set to Automatic.

If a HorizontalArrangement's Width property is set to Fill Parent or specified in pixels, any components whose Width properties are set to Fill Parent will equally take up the width not occupied by other components.

## Properties

### AlignHorizontal

A number that encodes how contents of the arrangement are aligned horizontally. The choices are: 1 = left aligned, 2 = right aligned, 3 = horizontally centered. Alignment has no effect if the arrangement's width is automatic.

### AlignVertical

A number that encodes how the contents of the arrangement are aligned vertically. The choices are: 1 = aligned at the top, 2 = aligned at the bottom, 3 = vertically centered. Alignment has no effect if the arrangement's height is automatic.

### BackgroundColor

Background color for this component

### Image

Background image for this component

### Visible

If true, component and its contents are visible.

### Height

Horizontal arrangement height \(y-size\).

### Width

Horizontal arrangement width \(x-size\).


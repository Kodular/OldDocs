# Slider

A Slider is a progress bar that adds a draggable thumb. You can touch the thumb and drag left or right to set the slider thumb position. As the Slider thumb is dragged, it will trigger the PositionChanged event, reporting the position of the Slider thumb. The reported position of the Slider thumb can be used to dynamically update another component attribute, such as the font size of a TextBox or the radius of a Ball.

## Properties

### ColorLeft

The color of slider to the left of the thumb.

### ColorRight

The color of slider to the left of the thumb.

### MaxValue

Sets the maximum value of slider. Changing the maximum value also resets Thumbposition to be halfway between the minimum and the \(new\) maximum. If the new maximum is less than the current minimum, then minimum and maximum will both be set to this value. Setting MaxValue resets the thumb position to halfway between MinValue and MaxValue and signals the PositionChanged event.

### MinValue

Sets the minimum value of slider. Changing the minimum value also resets Thumbposition to be halfway between the \(new\) minimum and the maximum. If the new minimum is greater than the current maximum, then minimum and maximum will both be set to this value. Setting MinValue resets the thumb position to halfway between MinValue and MaxValue and signals the PositionChanged event.

### ThumbPosition

Sets the position of the slider thumb. If this value is greater than MaxValue, then it will be set to same value as MaxValue. If this value is less than MinValue, then it will be set to same value as MinValue.

### ThumbEnabled

Sets whether or not to display the slider thumb.

### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

### Width

## Events

### PositionChanged\(number thumbPosition\)

Indicates that position of the slider thumb has changed.

## Methods

none


# List View

This is a visible component that allows to place a list of text elements in your Screen to display.  
The list can be set using the ElementsFromString property or using the Elements block in the blocks editor.  
Warning: This component will not work correctly on Screens that are scrollable.

## Properties

### BackgroundColor

The color of the listview background.

### Elements

List of text elements to build your list.

### ElementsFromString

Build a list with a series of text elements separated by commas such as: Cheese,Fruit,Bacon,Radish. Each word before the comma will be an element in the list.

### Height

Determines the height of the list on the view.

### Selection

Returns the text last selected in the ListView.

### SelectionIndex

The index of the currently selected item, starting at 1. If no item is selected, the value will be 0. If an attempt is made to set this to a number less than 1 or greater than the number of items in the ListView, SelectionIndex will be set to 0, and Selection will be set to the empty text.

### ShowFilterBar

Sets visibility of ShowFilterBar. True will show the bar, False will hide it.

### TextColor

The text color of the listview items.

### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

### Width

Determines the width of the list on the view.

## Events

### AfterPicking\(\)

Simple event to be raised after the an element has been chosen in the list. The selected element is available in the Selection property.

## Methods

none


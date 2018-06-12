# Spinner

A spinner component that displays a pop-up with a list of elements. These elements can be set in the Designer or Blocks Editor by setting theElementsFromString property to a string-separated concatenation \(for example, choice 1, choice 2, choice 3\) or by setting the Elements property to a List in the Blocks editor. Spinners are created with the first item already selected. So selecting it does not generate an After Picking event. Consequently it's useful to make the first Spinner item be a non-choice like "Select from below...".

## Properties

### Elements

returns a list of text elements to be picked from.

### ElementsFromString

sets the Spinner list to the elements passed in the comma-separated string

### Height

### Prompt

Text with the current title for the Spinner window

### Selection

Returns the current selected item in the spinner

### SelectionIndex

The index of the currently selected item, starting at 1. If no item is selected, the value will be 0.

### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

### Width

## Events

### AfterSelecting\(text selection\)

Event called after the user selects an item from the dropdown list.

## Methods

### DisplayDropdown\(\)

displays the dropdown list for selection, same action as when the user clicks on the spinner.


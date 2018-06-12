---
description: >-
  A button that, when clicked on, displays a list of texts for the user to
  choose among.
---

# List Picker

The texts can be specified through the Designer or Blocks Editor by setting the ElementsFromString property to their string-separated concatenation \(for example, choice 1, choice 2, choice 3\) or by setting the Elements property to a List in the Blocks editor.

Setting property ShowFilterBar to true, will make the list searchable. Other properties affect the appearance of the button \(TextAlignment, BackgroundColor, etc.\) and whether it can be clicked on \(Enabled\).

## Properties

### BackgroundColor

Returns the button's background color

### Elements

List of Choices to Display \(as a list\)

### ElementsFromString

Comma separated list of choices to use

### Enabled

Whether the ListPicker can be tapped

### FontBold \(designer only\)

If set, list picker text is displayed in bold.

### FontItalic \(designer only\)

If set, list picker text is displayed in italics.

### FontSize \(designer only\)

Point size for list picker text.

### FontTypeface \(designer only\)

Font family for list picker text.

### Height

Box height \(y-size\).

### Image

Specifies the path of the button's image. If there is both an Image and a BackgroundColor, only the Image will be visible.

### Selection

The selected item. When directly changed by the programmer, the SelectionIndex property is also changed to the first item in the ListPicker with the given value. If the value does not appear, SelectionIndex will be set to 0.

### SelectionIndex

The index of the currently selected item, starting at 1. If no item is selected, the value will be 0. If an attempt is made to set this to a number less than 1 or greater than the number of items in the ListPicker, SelectionIndex will be set to 0, and Selection will be set to the empty text.

### Shape \(designer only\)

Specifies the button's shape \(default, rounded, rectangular, oval\). The shape will not be visible if an Image is being displayed.

### ShowFeedback

Specifies if a visual feedback should be shown for a button that as an image as background.

### ShowFilterBar

Returns current state of ShowFilterBar indicating if Search Filter Bar will be displayed on ListPicker or not

### Text

Title text to display on list picker.

### TextAlignment \(designer only\)

Left, center, or right.

### TextColor

Color for text.

### Title

Optional title displayed at the top of the list of choices.

### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

### Width

Box width \(x-size\).

### ItemTextColor

The text color of the ListPicker items.

### ItemBackgroundColor

The background color of the ListPicker items.

## Events

### AfterPicking

Event to be raised after the picker activity returns its result and the properties have been filled in.

### BeforePicking

Event to raise when the button of the component is clicked or the list is shown using the Open block. This event occurs before the list of items is displayed, and can be used to prepare the list before it is shown.

### GotFocus

Indicates the cursor moved over the button so it is now possible to click it.

### LostFocus

Indicates the cursor moved away from the button so it is now no longer possible to click it.

## Methods

### Open

Opens the picker, as though the user clicked on it.


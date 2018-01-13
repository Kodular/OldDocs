# Ev3ColorSensor

A component that provides a high-level interface to a color sensor on a LEGO MINDSTORMS EV3 robot.

---

### Properties

#### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

#### SensorPort

The sensor port that the sensor is connected to. Must be set in the Designer

#### BottomOfRange

The bottom of the range used for the BelowRange, WithinRange, and AboveRange events.

#### TopOfRange

The top of the range used for the BelowRange, WithinRange, and AboveRange events.

#### BelowRangeEventEnabled

Whether the BelowRange event should fire when the light level goes below the BottomOfRange.

#### WithinRangeEventEnabled

Whether the WithinRange event should fire when the light level goes between the BottomOfRange and the TopOfRange.

#### AboveRangeEventEnabled

Whether the AboveRange event should fire when the light level goes above the TopOfRange.

#### ColorChangedEventEnabled

Whether the ColorChanged event should fire when the Mode property is set to "color" and the detected color changes.

#### Mode

Get the current sensor mode.

---

### Methods

#### GetLightLevel ()

It returns the light level in percentage, or -1 when the light level cannot be read.

#### GetColorCode ()

It returns the color code from 0 to 7 corresponding to no color, black, blue, green, yellow, red, white and brown.

#### GetColorName ()

Return the color name in one of "No Color", "Black", "Blue", "Green", "Yellow", "Red", "White", "Brown".

#### SetColorMode ()

Enter the color detection mode.

#### SetReflectedMode ()

Make the sensor read the light level with reflected light.

#### SetAmbientMode ()

Make the sensor read the light level without reflected light.

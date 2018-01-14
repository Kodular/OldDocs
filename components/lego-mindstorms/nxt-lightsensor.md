# NXT Light Sensor

A component that provides a high-level interface to a light sensor on a LEGO MINDSTORMS NXT robot

---

### Properties

#### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

#### SensorPort

The sensor port that the sensor is connected to. Must be set in the Designer

#### GenerateLight

Whether the light sensor should generate light.

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

---

### Events

#### BelowRange()

Light level has gone below the range.

#### WithinRange()

Light level has gone within the range.

#### AboveRange()

Light level has gone above the range.

---

### Methods

#### GetLightLevel ()

Returns the current light level as a value between 0 and 1023, or -1 if the light level can not be read.

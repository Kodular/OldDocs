# NXT Sound Sensor

A component that provides a high-level interface to a sound sensor on a LEGO MINDSTORMS NXT robot

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

Whether the BelowRange event should fire when the sound level goes below the BottomOfRange.

#### WithinRangeEventEnabled

Whether the WithinRange event should fire when the sound level goes between the BottomOfRange and the TopOfRange.

#### AboveRangeEventEnabled

Whether the AboveRange event should fire when the sound level goes above the TopOfRange.

---

### Events

#### BelowRange()

Sound level has gone below the range.

#### WithinRange()

Sound level has gone within the range.

#### AboveRange()

Sound level has gone above the range.

---

Methods

#### GetSoundLevel ()

Returns the current sound level as a value between 0 and 1023, or -1 if the sound level can not be read.

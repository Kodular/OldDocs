# NXT Ultrasonic Sensor

A component that provides a high-level interface to an ultrasonic sensor on a LEGO MINDSTORMS NXT robot

## Properties

### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

### SensorPort

The sensor port that the sensor is connected to. Must be set in the Designer

### BottomOfRange

The bottom of the range used for the BelowRange, WithinRange, and AboveRange events.

### TopOfRange

The top of the range used for the BelowRange, WithinRange, and AboveRange events.

### BelowRangeEventEnabled

Whether the BelowRange event should fire when the distance goes below the BottomOfRange.

### WithinRangeEventEnabled

Whether the WithinRange event should fire when the distance goes between the BottomOfRange and the TopOfRange.

### AboveRangeEventEnabled

Whether the AboveRange event should fire when the distance goes above the TopOfRange.

## Events

### BelowRange\(\)

Distance has gone below the range.

### WithinRange\(\)

Distance has gone within the range.

### AboveRange\(\)

Distance has gone above the range.

Methods

### GetDistance \(\)

Returns the current distance in centimeters as a value between 0 and 254, or -1 if the distance can not be read.


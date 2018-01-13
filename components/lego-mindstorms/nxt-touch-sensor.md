# NXT Touch Sensor

A component that provides a high-level interface to a touch sensor on a LEGO MINDSTORMS NXT robot

---

### Properties

#### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

#### SensorPort

The sensor port that the sensor is connected to. Must be set in the Designer

#### PressedEventEnabled

Whether the Pressed event should fire when the touch sensor is pressed.

#### ReleasedEventEnabled

Whether the Released event should fire when the touch sensor is released.

---

### Events

#### Pressed()

Touch sensor has been pressed.

#### Released()

Touch sensor has been released.

---

### Methods

#### IsPressed ()

Returns true if the touch sensor is pressed.

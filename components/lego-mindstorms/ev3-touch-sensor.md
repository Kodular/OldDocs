# Ev3TouchSensor

A component that provides a high-level interface to a touch sensor on a LEGO MINDSTORMS EV3 robot.

---

### Properties

#### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

#### SensorPort

The sensor port that the sensor is connected to. Must be set in the Designer

#### PressedEventEnabled

Whether the Released event should fire when the touch sensor is pressed.

#### ReleasedEventEnabled

Whether the Released event should fire when the touch sensor is released.

---

### Methods

#### IsPressed ()

Returns true if the touch sensor is pressed.

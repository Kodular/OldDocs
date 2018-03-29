# EV3 Gyro Sensor

A component that provides a high-level interface to a gyro sensor on a LEGO MINDSTORMS EV3 robot.

## Properties

### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

### SensorPort

The sensor port that the sensor is connected to. Must be set in the Designer

### Mode

The sensor mode can be a text constant of either "rate" or "angle", which correspond to SetAngleMode or SetRateMode respectively.

### SensorValueChangedEventEnabled

Whether the SensorValueChanged event should fire when the sensor value changed.

## Methods

### GetSensorValue \(\)

Returns the current angle or rotation speed based on current mode, or -1 if the value cannot be read from sensor.

### SetAngleMode \(\)

Measures the orientation of the sensor.

### SetRateMode \(\)

Measures the angular velocity of the sensor.


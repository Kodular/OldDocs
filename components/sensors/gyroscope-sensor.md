# Gyroscope Sensor

Non-visible component that can measure angular velocity in three dimensions in units of degrees per second.

In order to function, the component must have its Enabled property set to True, and the device must have a gyroscope sensor.

## Properties

### Available

Indicates whether a gyroscope sensor is available.

### Enabled

If enabled, then sensor events will be generated and XAngularVelocity, YAngularVelocity, and ZAngularVelocity properties will have meaningful values.

### XAngularVelocity

The angular velocity around the X axis, in degrees per second.

### YAngularVelocity

The angular velocity around the Y axis, in degrees per second.

### ZAngularVelocity

The angular velocity around the Z axis, in degrees per second.

## Events

### GyroscopeChanged\(number xAngularVelocity, number yAngularVelocity, number zAngularVelocity, number timestamp\)

Indicates that the gyroscope sensor data has changed. The timestamp parameter is the time in nanoseconds at which the event occurred.

## Methods

none


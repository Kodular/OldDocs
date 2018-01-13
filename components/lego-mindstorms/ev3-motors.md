# Ev3Motors

A component that provides both high- and low-level interfaces to a LEGO MINDSTORMS EV3 robot, with functions that can control the motors.

---

### Properties

#### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

#### MotorPorts

The motor ports that the motors are connected to. The ports are specified by a sequence of port letters. Must be set in the Designer

#### WheelDiameter

The diameter of the wheels attached on the motors in centimeters.

#### ReverseDirection

It specifies if the direction of the motors is reversed.

#### EnableSpeedRegulation

The robot adjusts the power to maintain the speed if speed regulation is enabled.

#### StopBeforeDisconnect

Whether to stop the motor before disconnecting.

#### TachoCountChangedEventEnabled

Whether the TachoCountChanged event should fire when the angle is changed.

---

### Methods

#### RotateIndefinitely (number power)

Start to rotate the motors.

#### RotateInTachoCounts (number power, number tachoCounts, boolean useBrake)

Rotate the motors in a number of tacho counts.

#### RotateInDuration (number power, number milliseconds, boolean useBrake)

Rotate the motors in a period of time.

#### RotateInDistance (number power, number distance, boolean useBrake)

Rotate the motors in a distance.

#### RotateSyncIndefinitely (number power, number turnRatio)

Start to rotate the motors at the same speed.

#### RotateSyncInDistance (number power, number distance, number turnRatio, boolean useBrake)

Rotate the motors at the same speed for a distance in cm.

#### RotateSyncInDuration (number power, number milliseconds, number turnRatio, boolean useBrake)

Rotate the motors at the same speed in a period of time.

#### RotateSyncInTachoCounts (number power, number tachoCounts, number turnRatio, boolean useBrake)

Rotate the motors at the same speed in a number of tacho counts.

#### Stop (boolean useBrake)

Stop the motors of the robot.

#### ToggleDirection ()

Toggle the direction of motors.

#### ResetTachoCount ()

Set the current tacho count to zero.

#### GetTachoCount ()

Get the current tacho count.

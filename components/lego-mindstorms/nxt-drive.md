# NXT Drive

A component that provides a high-level interface to a LEGO MINDSTORMS NXT robot, with functions that can move and turn the robot

---

### Properties

#### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

#### DriveMotors

The motor ports that are used for driving.

#### WheelDiameter

The diameter of the wheels used for driving.

#### StopBeforeDisconnect

Whether to stop the drive motors before disconnecting.

---

### Methods

#### MoveForwardIndefinitely (number power)

Move the robot forward indefinitely, with the specified percentage of maximum power.

#### MoveForward (number power, number distance)

Move the robot forward the given distance, with the specified percentage of maximum power.

#### MoveBackwardIndefinitely (number power)

Move the robot backward indefinitely, with the specified percentage of maximum power.

#### MoveBackward (number power, number distance)

Move the robot backward the given distance, with the specified percentage of maximum power.

#### Stop ()

Stop the drive motors of the robot.

#### TurnClockwiseIndefinitely (number power)

Turn the robot clockwise indefinitely, with the specified percentage of maximum power.

#### TurnCounterClockwiseIndefinitely (number power)

Turn the robot counterclockwise indefinitely, with the specified percentage of maximum power.

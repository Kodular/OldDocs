# NXT Direct Commands

A component that provides a low-level interface to a LEGO MINDSTORMS NXT robot, with functions to send NXT Direct Commands

---

### Properties

#### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

---

### Methods

#### DeleteFile (text fileName)

Delete a file on the robot.

#### DownloadFile (text source, text destination)

Download a file to the robot.

#### GetBatteryLevel ()

Get the battery level for the robot. Returns the voltage in millivolts.

#### GetBrickName ()

Get the brick name of the robot.

#### GetCurrentProgramName ()

Get the name of currently running program on the robot.

#### GetFirmwareVersion ()

Get the firmware and protocol version numbers for the robot as a list where the first element is the firmware version number and the second element is the protocol version number.

#### GetInputValues (text sensorPortLetter)

Reads the values of an input sensor on the robot. Assumes sensor type has been configured via SetInputMode.

#### GetOutputState (text motorPortLetter)

Reads the output state of a motor on the robot.

#### KeepAlive ()

Keep Alive. Returns the current sleep time limit in milliseconds.

#### ListFiles (text wildcard)

Returns a list containing the names of matching files found on the robot.

#### LsGetStatus (text sensorPortLetter)

Returns the count of available bytes to read.

#### LsRead (text sensorPortLetter)

Reads unsigned low speed data from an input sensor on the robot. Assumes sensor type has been configured via SetInputMode.

#### LsWrite (text sensorPortLetter, list list, number rxDataLength)

Writes low speed data to an input sensor on the robot. Assumes sensor type has been configured via SetInputMode.

#### MessageRead (number mailbox)

Read a message from a mailbox (1-10) on the robot.

#### MessageWrite (number mailbox, text message)

Write a message to a mailbox (1-10) on the robot.

#### PlaySoundFile (text fileName)

Play a sound file on the robot.

#### PlayTone (number frequencyHz, number durationMs)

Make the robot play a tone.

#### ResetInputScaledValue (text sensorPortLetter)

Reset the scaled value of an input sensor on the robot.

#### ResetMotorPosition (text motorPortLetter, boolean relative)

Reset motor position.

#### SetBrickName (text name)

Set the brick name of the robot.

#### SetInputMode (text sensorPortLetter, number sensorType, number sensorMode)

Configure an input sensor on the robot.

#### SetOutputState (text motorPortLetter, number power, number mode, number regulationMode, number turnRatio, number runState, number tachoLimit)

Sets the output state of a motor on the robot.

#### StartProgram (text programName)

Start execution of a previously downloaded program on the robot.

#### StopProgram ()

Stop execution of the currently running program on the robot.

#### StopSoundPlayback ()

Stop sound playback.

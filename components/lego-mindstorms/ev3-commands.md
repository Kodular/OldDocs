# Ev3Commands

A component that provides a low-level interface to a LEGO MINDSTORMS EV3 robot, with functions to send system or direct commands to EV3 robots.

---

### Properties

#### BluetoothClient

The BluetoothClient component that should be used for communication. Must be set in the Designer

---

### Methods

#### KeepAlive (number minutes)

Keep the EV3 brick from shutdown for a period of time.

#### GetBatteryVoltage ()

Get the battery voltage.

#### GetBatteryCurrent ()

Get the battery current.

#### GetOSVersion ()

Get the OS version on EV3.

#### GetOSBuild ()

Get the OS build on EV3.

#### GetFirmwareVersion ()

Get the firmware version on EV3.

#### GetFirmwareBuild ()

Get the firmware build on EV3.

#### GetHardwareVersion ()

Get the hardware version of EV3.

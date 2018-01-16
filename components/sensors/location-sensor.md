# LocationSensor

Non-visible component providing location information, including longitude, latitude, altitude (if supported by the device), speed (if supported by the device), and address. This can also perform "geocoding", converting a given address (not necessarily the current one) to a latitude (with the LatitudeFromAddress method) and a longitude (with the LongitudeFromAddress method).

In order to function, the component must have its Enabled property set to True, and the device must have location sensing enabled through wireless networks or GPS satellites (if outdoors).

Location information might not be immediately available when an app starts. You'll have to wait a short time for a location provider to be found and used, or wait for the OnLocationChanged event.

---

### Properties

#### Accuracy

#### Altitude

#### AvailableProviders

#### CurrentAddress

#### DistanceInterval

Determines the minimum distance interval, in meters, that the sensor will try to use for sending out location updates. For example, if this is set to 5, then the sensor will fire a LocationChanged event only after 5 meters have been traversed. However, the sensor does not guarantee that an update will be received at exactly the distance interval. It may take more than 5 meters to fire an event, for instance.

#### Enabled

#### HasAccuracy

#### HasAltitude

#### HasLongitudeLatitude

#### Latitude

#### Longitude

#### ProviderLocked

#### ProviderName

#### TimeInterval

Determines the minimum time interval, in milliseconds, that the sensor will try to use for sending out location updates. However, location updates will only be received when the location of the phone actually changes, and use of the specified time interval is not guaranteed. For example, if 1000 is used as the time interval, location updates will never be fired sooner than 1000ms, but they may be fired anytime after.

---

### Events

#### LocationChanged(number latitude, number longitude, number altitude, number speed)

Indicates that a new location has been detected.

#### StatusChanged(text provider, text status)

Indicates that the status of the location provider service has changed, such as when a provider is lost or a new provider starts being used.

---

### Methods

#### LatitudeFromAddress(text locationName)

Derives latitude of given address

#### LongitudeFromAddress(text locationName)

Derives longitude of given address

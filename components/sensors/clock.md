# Clock

Non-visible component that provides the instant in time using the internal clock on the phone.It can fire a timer at regularly set intervals and perform time calculations, manipulations, and conversions.

Methods to convert an instant to text are also available. Acceptable patterns are empty string, MM/DD/YYYY HH:mm:ss a, or MMM d, yyyy HH:mm. The empty string will provide the default format, which is "MMM d, yyyy HH:mm:ss a" for FormatDateTime, "MMM d, yyyy" for FormatDate. To see all possible format, please see here.

Date and Time are formatted with InstantInTime and Duration.

Instant : consists of Year, Month, DayOfMonth, Hour, Minute, and Second. An instant can be created by using MakeInstant method.

Duration : time in milliseconds elapsed between instants. Duration can be obtained by Duration method.

## Properties

### TimerAlwaysFires

Will fire even when application is not showing on the screen if true

### TimerEnabled

Fires timer if true

### TimerInterval

Interval between timer events in ms

## Events

### Timer\(\)

Timer has gone off.

## Methods

### InstantInTime AddDays\(InstantInTime instant, number days\)

Returns an instant in time some days after the argument

### InstantInTime AddDuration\(InstantInTime instant, Duration duration\)

Returns an instant in time some time after the argument. Duration can be obtained from Clock.Duration\(\)

### InstantInTime AddHours\(InstantInTime instant, number hours\)

Returns an instant in time some hours after the argument

### InstantInTime AddMinutes\(InstantInTime instant, number minutes\)

Returns an instant in time some minutes after the argument

### InstantInTime AddMonths\(InstantInTime instant, number months\)

Returns an instant in time some months after the argument

### InstantInTime AddSeconds\(InstantInTime instant, number seconds\)

Returns an instant in time some seconds after the argument

### InstantInTime AddWeeks\(InstantInTime instant, number weeks\)

Returns an instant in time some weeks after the argument

### InstantInTime AddYears\(InstantInTime instant, number years\)

Returns an instant in time some years after the argument

### DayOfMonth\(InstantInTime instant\)

Returns the day of the month\(1-31\) from the instant

### Duration\(InstantInTime start, InstantInTime end\)

Returns duration, which is milliseconds elapsed between instants

### DurationToSeconds\(Duration duration\)

Converts the duration to the number of seconds.

### DurationToMinutes\(Duration duration\)

Converts the duration to the number of minutes.

### DurationToHours\(Duration duration\)

Converts the duration to the number of hours.

### DurationToDays\(Duration duration\)

Converts the duration to the number of days.

number DurationToWeeks\(Duration duration\)

Converts the duration to the number of weeks.

### FormatDate\(InstantInTime instant, text pattern\)

Returns text representing the date of an instant in the specified pattern

### FormatDateTime\(InstantInTime instant, text pattern\)

Returns text representing the date and time of an instant in the specified pattern

### FormatTime\(InstantInTime instant\)

Return text representing the time of an instant

### GetMillis\(InstantInTime instant\)

Returns the instant in time measured as milliseconds since 1970.

### Hour\(InstantInTime instant\)

Returns the hour of the day\(0-23\) from the instant

### InstantInTime MakeInstant\(text from\)

Returns an instant specified by MM/DD/YYYY hh:mm:ss or MM/DD/YYYY or hh:mm. An example text input is "06/22/2015 12:18"

### InstantInTime MakeInstantFromMillis\(number millis\)

Returns an instant in time specified by the milliseconds since 1970.

### Minute\(InstantInTime instant\)

Returns the minute of the hour \(0-59\) from the instant

### Month\(InstantInTime instant\)

Returns the month of the year \(1-12\) from the instant

### MonthName\(InstantInTime instant\)

Returns the name of the month from the instant E.g. January, February, March...

### InstantInTime Now\(\)

Returns an instant of the current time read from phone's clock

### Second\(InstantInTime instant\)

Returns the second of the minute \(0-59\) from the instant

### SystemTime\(\)

Returns the phone's internal time

### Weekday\(InstantInTime instant\)

Returns the day of the week represented as a number from 1 \(Sunday\) to 7 \(Saturday\)

### WeekdayName\(InstantInTime instant\)

Returns the name of the day of the week from the instant

### Year\(InstantInTime instant\)

Returns the year from the instant


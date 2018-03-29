# Pedometer

A Component that acts like a Pedometer. It senses motion via the Accerleromter and attempts to determine if a step has been taken. Using a configurable stride length, it can estimate the distance traveled as well.

## Properties

### Distance

The approximate distance traveled in meters.

### ElapsedTime

Time elapsed in milliseconds since the pedometer was started.

### SimpleSteps

The number of simple steps taken since the pedometer has started.

### StopDetectionTimeout

The duration in milliseconds of idleness \(no steps detected\) after which to go into a "stopped" state

### StrideLength

Set the average stride length in meters.

### WalkSteps

the number of walk steps taken since the pedometer has started.

## Events

### SimpleStep\(number simpleSteps, number distance\)

This event is run when a raw step is detected

### WalkStep\(number walkSteps, number distance\)

This event is run when a walking step is detected. A walking step is a step that appears to be involved in forward motion.

## Methods

### Pause\(\)

Pause counting of steps and distance.

### Reset\(\)

Resets the step counter, distance measure and time running.

### Resume\(\)

Resumes counting, synonym of Start.

### Save\(\)

Saves the pedometer state to the phone. Permits permits accumulation of steps and distance between invocations of an App that uses the pedometer. Different Apps will have their own saved state.

### Start\(\)

Start counting steps

### Stop\(\)

Stop counting steps


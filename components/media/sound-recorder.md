# Sound Recorder

Multimedia component that records audio.

---

### Properties

#### SavedRecording

Specifies the path to the file where the recording should be stored. If this proprety is the empty string, then starting a recording will create a file in an appropriate location. If the property is not the empty string, it should specify a complete path to a file in an existing directory, including a file name with the extension .3gp.

---

### Events

#### AfterSoundRecorded(text sound)

Provides the location of the newly created sound.

#### StartedRecording()

Indicates that the recorder has started, and can be stopped.

#### StoppedRecording()

Indicates that the recorder has stopped, and can be started again.

---

### Methods

#### Start ()

Starts recording.

#### Stop ()

Stops recording.

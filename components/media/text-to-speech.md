# Text To Speech

The TextToSpeech component speaks a given text aloud. You can set the pitch and the rate of speech.

You can also set a language by supplying a language code. This changes the pronounciation of words, not the actual language spoken. For example, setting the language to French and speaking English text will sound like someone speaking English \(en\) with a French accent.

You can also specify a country by supplying a country code. This can affect the pronounciation. For example, British English \(GBR\) will sound different from US English \(USA\). Not every country code will affect every language.

The languages and countries available depend on the particular device, and can be listed with the AvailableLanguages and AvailableCountries properties.

## Properties

### AvailableCountries

List of the country codes available on this device for use with TextToSpeech. Check the Android developer documentation under supported languages to find the meanings of these abbreviations.

### AvailableLanguages

List of the languages available on this device for use with TextToSpeech. Check the Android developer documentation under supported languages to find the meanings of these abbreviations.

### Country

Country code to use for speech generation. This can affect the pronounciation. For example, British English \(GBR\) will sound different from US English \(USA\). Not every country code will affect every language.

### Language

Sets the language for TextToSpeech. This changes the way that words are pronounced, not the actual language that is spoken. For example setting the language to French and speaking English text will sound like someone speaking English with a French accent.

### Pitch

Sets the Pitch for TextToSpeech. The values should be between 0 and 2 where lower values lower the tone of synthesized voice and greater values raise it.

### Result

### SpeechRate

Sets the SpeechRate for TextToSpeech. The values should be between 0 and 2 where lower values slow down the pitch and greater values accelerate it.

## Events

### AfterSpeaking\(boolean result\)

Event to raise after the message is spoken.

### BeforeSpeaking\(\)

Event to raise when Speak is invoked, before the message is spoken.

## Methods

### Speak\(text message\)

Speaks the given message.


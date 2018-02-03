# Firebase DB

A non-visible component allowing you to store data on an online Realtime Database powered by Firebase.

---

### Properties

#### Firebase Token

A valid Legacy Database Secret of the Database with which to connect.

#### Firebase URL

The URL of the Database with which to connect.

#### Use Default

Check to use default Firebase Database.

#### Persist


#### App Bucket

The bucket in the Database in which all operations on Data should take place.

---

### Events

#### DataChanged(text tag, any value)

Indicates that data has been modified in the Firebase Database.

#### FirebaseError(text message)

Indicates that the Firebase Database had an error.

#### FirstRemoved(any value)

#### GotValue(text tag, any value)

Indicates that a piece of data has been successfully retrieved.

#### TagList(list value)

Indicates that the list of tags has been fetched.

---

### Methods

#### AppendValue(text tag any value)

Adds a new value to the existing value stored in a tag.

#### ClearTag(text tag)

Deletes a tag from the Firebase Database.

#### GetTagList()

Fetches the list of tags in the Firebase Database

#### GetValue(text tag any valueIfTagNotThere)

Fetches the value stored in a tag. Returns valueIfTagNotThere if the tag is not present in the Firebase Database.

#### GoOffline()

Stops interacting with the Firebase Database.

#### GoOnline()

Starts interacting with the Firebase Database.

#### RemoveFirst(text tag)

#### StoreValue(text tag, any valueToStore)

Stores valueToStore in a tag in the Firebase Database

#### Unauthenticate()

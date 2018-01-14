# Tiny DB

TinyDB is a non-visible component that stores data for an app.

Apps created with App Inventor are initialized each time they run. This means that if an app sets the value of a variable and the user then quits the app, the value of that variable will not be remembered the next time the app is run. In contrast, TinyDB is a persistent data store for the app. The data stored in a TinyDB will be available each time the app is run. An example might be a game that saves the high score and retrieves it each time the game is played.

Data items are strings stored under tags. To store a data item, you specify the tag it should be stored under. Subsequently, you can retrieve the data that was stored under a given tag.

Each app has its own data store. There is only one data store per app. Even if you have multiple TinyDB components, they will use the same data store. To get the effect of separate stores, use different keys. You cannot use the TinyDB to pass data between two different apps on the phone, although you can use the TinyDB to share data between the different screens of a multi-screen app.

When you are developing apps using the AI Companion, all the apps using that Companion will share the same TinyDB. That sharing will disappear once the apps are packaged and installed on the phone. During development you should be careful to clear the Companion app's data each time you start working on a new app.

---

### Properties

none

---

### Events

none

---

### Methods

#### ClearAll()

Clear the entire data store in the TinyDB.

#### ClearTag(text tag)

Clear the entry with the given tag.

#### any GetTags()

Return a list of all the tags in the TinyDB.

#### any GetValue(text tag, any valueIfTagNotThere)

Retrieve the value stored under the given tag. If there's no such tag, then return valueIfTagNotThere.

#### StoreValue(text tag, any valueToStore)

Store the value under the given tag. The storage persists on the phone when the app is restarted.

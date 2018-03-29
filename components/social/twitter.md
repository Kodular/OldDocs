# Twitter

A non-visible component that enables communication with Twitter. Once a user has logged into their Twitter account \(and the authorization has been confirmed successful by the IsAuthorized event\), many more operations are available:

* Searching Twitter for tweets or labels \(SearchTwitter\)
* Sending a Tweet \(Tweet\)
* Sending a Tweet with an Image \(TweetWithImage\)
* Directing a message to a specific user \(DirectMessage\)
* Receiving the most recent messages directed to the logged-in user \(RequestDirectMessages\)
* Following a specific user \(Follow\)
* Ceasing to follow a specific user \(StopFollowing\)
* Getting a list of users following the logged-in user \(RequestFollowers\)
* Getting the most recent messages of users followed by the logged-in user \(RequestFriendTimeline\)
* Getting the most recent mentions of the logged-in user \(RequestMentions\)

You must obtain a Consumer Key and Consumer Secret for Twitter authorization specific to your app from [http://twitter.com/oauth\_clients/new](http://twitter.com/oauth_clients/new)

## Properties

### ConsumerKey

The consumer key to be used when authorizing with Twitter via OAuth.

### ConsumerSecret

The consumer secret to be used when authorizing with Twitter via OAuth

### DirectMessages

This property contains a list of the most recent messages mentioning the logged-in user. Initially, the list is empty. To set it, the program must:

* Call the Authorize method.
* Wait for the Authorized event.
* Call the RequestDirectMessages method.
* Wait for the DirectMessagesReceived event.

The value of this property will then be set to the list of direct messages retrieved \(and maintain that value until any subsequent call to RequestDirectMessages\).

### Followers

This property contains a list of the followers of the logged-in user. Initially, the list is empty. To set it, the program must:

* Call the Authorize method.
* Wait for the IsAuthorized event.
* Call the RequestFollowers method.
* Wait for the FollowersReceived event.

The value of this property will then be set to the list of followers \(and maintain its value until any subsequent call to RequestFollowers\).

### FriendTimeline

This property contains the 20 most recent messages of users being followed. Initially, the list is empty. To set it, the program must:

* Call the Authorize method.
* Wait for the IsAuthorized event.
* Specify users to follow with one or more calls to the Follow method.
* Call the RequestFriendTimeline method.
* Wait for the FriendTimelineReceived event.

The value of this property will then be set to the list of messages \(and maintain its value until any subsequent call to RequestFriendTimeline.

### Mentions

This property contains a list of mentions of the logged-in user. Initially, the list is empty. To set it, the program must:

* Call the Authorize method.
* Wait for the IsAuthorized event.
* Call the RequestMentions method.
* Wait for the MentionsReceived event.

The value of this property will then be set to the list of mentions \(and will maintain its value until any subsequent calls to RequestMentions\).

### SearchResults

This property, which is initially empty, is set to a list of search results after the program:

* Calls the SearchTwitter method.
* Waits for the SearchSuccessful event.
* The value of the property will then be the same as the parameter to SearchSuccessful. Note that it is not necessary to call the Authorize method before calling SearchTwitter.

### Username

The user name of the authorized user. Empty if there is no authorized user.

## Events

### DirectMessagesReceived\(list messages\)

This event is raised when the recent messages requested through RequestDirectMessages have been retrieved. A list of the messages can then be found in the messages parameter or the Messages property.

### FollowersReceived\(list followers2\)

This event is raised when all of the followers of the logged-in user requested through RequestFollowers have been retrieved. A list of the followers can then be found in the followers parameter or the Followers property.

### FriendTimelineReceived\(list timeline\)

This event is raised when the messages requested through RequestFriendTimeline have been retrieved. The timeline parameter and the Timeline property will contain a list of lists, where each sub-list contains a status update of the form \(username message\)

### IsAuthorized\(\)

This event is raised after the program calls Authorize if the authorization was successful. It is also called after a call to CheckAuthorized if we already have a valid access token. After this event has been raised, any other method for this component can be called.

### MentionsReceived\(list mentions\)

This event is raised when the mentions of the logged-in user requested through RequestMentions have been retrieved. A list of the mentions can then be found in the mentions parameter or the Mentions property.

### SearchSuccessful\(list searchResults\)

This event is raised when the results of the search requested through SearchSuccessful have been retrieved. A list of the results can then be found in the results parameter or the Results property.

## Methods

### Authorize\(\)

Redirects user to login to Twitter via the Web browser using the OAuth protocol if we don't already have authorization.

### CheckAuthorized\(\)

Checks whether we already have access, and if so, causes IsAuthorized event handler to be called.

### DeAuthorize\(\)

Removes Twitter authorization from this running app instance

### DirectMessage\(text user, text message\)

This sends a direct \(private\) message to the specified user. The message will be trimmed if it exceeds 160characters.  
Requirements: This should only be called after the IsAuthorized event has been raised, indicating that the user has successfully logged in to Twitter.

### Follow\(text user\)

Starts following a user.

### RequestDirectMessages\(\)

Requests the 20 most recent direct messages sent to the logged-in user. When the messages have been retrieved, the system will raise the DirectMessagesReceived event and set the DirectMessages property to the list of messages.

Requirements: This should only be called after the IsAuthorized event has been raised, indicating that the user has successfully logged in to Twitter.

### RequestFollowers\(\)

Gets who is following you.

### RequestFriendTimeline\(\)

Gets the most recent 20 messages in the user's timeline.

### RequestMentions\(\)

Requests the 20 most recent mentions of the logged-in user. When the mentions have been retrieved, the system will raise the MentionsReceived event and set the Mentions property to the list of mentions.

Requirements: This should only be called after the IsAuthorized event has been raised, indicating that the user has successfully logged in to Twitter.

### SearchTwitter\(text query\)

This searches Twitter for the given String query.

Requirements: This should only be called after the IsAuthorized event has been raised, indicating that the user has successfully logged in to Twitter.

### StopFollowing\(text user\)

Stops following a user.

### Tweet\(text status\)

This sends a tweet as the logged-in user with the specified Text, which will be trimmed if it exceeds 160 characters.  
Requirements: This should only be called after the IsAuthorized event has been raised, indicating that the user has successfully logged in to Twitter.

### TweetWithImage\(text status, text imagePath\)

This sends a tweet as the logged-in user with the specified Text and a path to the image to be uploaded, which will be trimmed if it exceeds 160 characters. If an image is not found or invalid, the update will not be sent.

Requirements: This should only be called after the IsAuthorized event has been raised, indicating that the user has successfully logged in to Twitter.


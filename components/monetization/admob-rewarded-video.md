# AdMob Rewarded Video

Rewarded video ads are full screen video ads that users have the option of watching in full in exchange for in-app rewards.

---

### Properties

##### AdEnabled

If true, device that will receive test ads. You should utilize this property during development to avoid generating false impressions

##### AdUnitId (designer only)

##### TestMode

For debugging/development purposes flag all ad requests as tests, but set to false for production builds. Will take effect when you use LoadAd block.

---

### Events

##### AdClosed

Called when the user is about to return to the application after clicking on an ad

##### AdFailedToLoad

| Parameter | Type |
| :--- | :--- |
| errCode | number |
| errMessage | text |

Triggered when AD fails to load

##### AdLeftApplication

Called when an ad leaves the application (e.g., to go to the browser).

##### AdLoaded

Called when an ad is received

##### AdOpened

Ad was opened by user

##### Rewarded

| Parameter | Type |
| :--- | :--- |
| type | text |
| amount | number |

User watched video and should be rewarded

---

### Methods

##### LoadAd

Loads a new ad.

##### ShowAd

It will show the Video

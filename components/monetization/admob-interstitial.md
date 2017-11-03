# AdMobInterstitial

An interstitial ad is a full-page ad. AdMob Interstitial component allows you to monetize your app. You must have a valid AdMob account and AdUnitId that can be obtained from http://www.google.com/AdMob . If your id is invalid, the AdMob Interstitial will not display on the emulator or the device. Warning: Make sure you're in test mode during development to avoid being disabled for clicking your own ads.

---

### Properties


##### AdEnabled

If true, device that will receive test ads. You should utilize this property during development to avoid generating false impressions

##### AdUnitID (designer only)


##### TargetAge

Leave 0 for targeting ALL ages

##### TargetForChildren

Indicate whether you want Google to treat your content as child-directed when you make an ad request. Info here: https://developers.google.com/mobile-ads-sdk/docs/admob/android/targeting#child-directed_setting

##### TargetGender


---

### Events

##### AdClosed

Called when the user is about to return to the application after clicking on an ad

##### AdFailedToLoad

| Parameter | Type |
| :--- | :--- |
| error | text |
| message | text |

Called when an ad request failed. message will display the reason for why the ad failed

##### AdFailedToShow

| Parameter | Type |
| :--- | :--- |
| message | text |

Called when an an attempt was made to display the ad, but the ad was not ready to display

##### AdLeftApplication

Called when an ad leaves the application (e.g., to go to the browser).

##### AdLoaded

Called when an ad is received

---

### Methods

##### LoadAd

Loads a new ad.

##### ShowInterstitialAd

It will show the Interstitial Ad
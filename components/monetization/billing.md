# Billing

In-App Purchases component by Pavitra.

---

### Properties

##### IsIabServiceAvailable

Check Play Market services availability

##### IsOneTimePurchaseSupported

Is One Time Purchase Supported

##### IsSubscriptionUpdateSupported

Is Subscription Update Supported

##### ReadyToPurchase

whether In-app billing service is ready to purchase

##### SuppressToast

whether Toast should be suppressed

##### TestMode

whether it is testing

---

### Events

##### AfterPurchase

| Parameter | Type |
| :--- | :--- |
| productId | text |

After purchase event.

##### ErrorOccurred

| Parameter | Type |
| :--- | :--- |
| message | text |

Error occurred event.

##### GotOwnedPurchases

| Parameter | Type |
| :--- | :--- |
| ownedProducts | list |
| ownedSubscriptions | list |

Got Owned Purchases

##### GotProductDetails

| Parameter | Type |
| :--- | :--- |
| success | boolean |
| productId | text |
| title | text |
| description | text |
| currency | text |
| price | text |

Got Product Details

##### GotSubscriptionDetails

| Parameter | Type |
| :--- | :--- |
| success | boolean |
| isSubscription | boolean |
| subscriptionId | text |
| title | text |
| description | text |
| currency | text |
| price | text |

Got Subscription Details

---

### Methods

##### Consume

| Parameter | Type |
| :--- | :--- |
| productId | text |

Consume product.

##### Initialize

| Parameter | Type |
| :--- | :--- |
| productId | text |
| licenseKey | text |
| merchantId | text |

Initialize Billing with License Key & Merchant ID

##### IsPurchased

###### Returns: (boolean)

| Parameter | Type |
| :--- | :--- |
| productId | text |

Is purchased?

##### IsSubscribed

###### Returns: (boolean)

| Parameter | Type |
| :--- | :--- |
| subscriptionId | text |

Is subscribed?

##### LoadOwnedPurchases

Load Owned Purchases from Google

##### ProductDetails

| Parameter | Type |
| :--- | :--- |
| productId | text |

Get Product Details.

##### Purchase

| Parameter | Type |
| :--- | :--- |
| productId | text |

Purchase product.

##### Subscribe

| Parameter | Type |
| :--- | :--- |
| subscriptionId | text |

Subscribe product.

##### SubscriptionDetails

| Parameter | Type |
| :--- | :--- |
| subscriptionId | text |

Get Subscription Details.

##### UpdateSubscription

| Parameter | Type |
| :--- | :--- |
| subscriptionId | text |

Update Subscription
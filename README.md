# app.tcs.ch

This repo allow domain validation for app.tcs.ch so it can be used for deeplinks to the TCS App. It provides the right configuration with the .well-known folder available on the domain with github pages.

### .well-known folder

The two files in the `.well-known` folder are used by both Android and iOS to verify the domain and deep-linking configurations.

| File name | Used by | Documentation |
| --- | --- | --- |
| `assetlinks.json` | Android | https://developer.android.com/training/app-links/verify-android-applinks?hl=fr#publish-json |
| `apple-app-site-association` | iOS | https://developer.apple.com/documentation/xcode/supporting-associated-domains |


### Redirections
Note that `index.html` and `404.html` both redirects to `tcs.ch/app` website in case the deeplink is not supported in user-device.

For example a user accessing `https://app.tcs.ch/map` on his computer would be redirected to the tcs website instead of seeing a generic 404 page.


### Contributing

Any commit on `main` will rebuild the github pages automatically

# FastlogsAuthSession

class FastlogsAuthSession(val context: [Activity](https://developer.android.com/reference/kotlin/android/app/Activity.html), val fastlogsConfig: [FastlogsConfig](../../io.fastlogs.sdk.android.type/-fastlogs-config/index.md), val oidcConfig: OidcConfigResponse, val redirectUri: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), completion: [Completion](../../io.fastlogs.sdk.android.completion/-completion/index.md)&lt;[FastlogsException](../../io.fastlogs.sdk.android.exception/-fastlogs-exception/index.md), CodeTokenResponse&gt;)

## Constructors

| Name             | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| FastlogsAuthSession | fun FastlogsAuthSession(context: [Activity](https://developer.android.com/reference/kotlin/android/app/Activity.html), fastlogsConfig: [FastlogsConfig](../../io.fastlogs.sdk.android.type/-fastlogs-config/index.md), oidcConfig: OidcConfigResponse, redirectUri: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), completion: [Completion](../../io.fastlogs.sdk.android.completion/-completion/index.md)&lt;[FastlogsException](../../io.fastlogs.sdk.android.exception/-fastlogs-exception/index.md), CodeTokenResponse&gt;) |

## Functions

| Name              | Summary                                                                                                        |
| ----------------- | -------------------------------------------------------------------------------------------------------------- |
| handleCallbackUri | fun handleCallbackUri(callbackUri: [Uri](https://developer.android.com/reference/kotlin/android/net/Uri.html)) |
| handleUserCancel  | fun handleUserCancel()                                                                                         |
| start             | fun start()                                                                                                    |

## Properties

| Name        | Summary                                                                                           |
| ----------- | ------------------------------------------------------------------------------------------------- |
| context     | val context: [Activity](https://developer.android.com/reference/kotlin/android/app/Activity.html) |
| fastlogsConfig | val fastlogsConfig: [FastlogsConfig](../../io.fastlogs.sdk.android.type/-fastlogs-config/index.md)            |
| oidcConfig  | val oidcConfig: OidcConfigResponse                                                                |
| redirectUri | val redirectUri: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

In Android, the Redirect URI follows the pattern: `$(FASTLOGS_REDIRECT_SCHEME)://$(YOUR_APP_PACKAGE)/callback`.

:::note
The `FASTLOGS_REDIRECT_SCHEME` should be a custom scheme in the reverse domain format.  
The `YOUR_APP_PACKAGE` is your app package name.
:::

Assuming you treat `io.fastlogs.android` as the custom `FASTLOGS_REDIRECT_SCHEME`, and `io.fastlogs.sample` is your app package name, the Redirect URI should be `io.fastlogs.android://io.fastlogs.sample/callback`.

Now you can configure the Redirect URI in the admin console (Take `io.fastlogs.android://io.fastlogs.sample/callback` as an example).

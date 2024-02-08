```kotlin
fastlogsClient.signIn(this, "<your-redirect-uri>") { fastlogsException: FastlogsException? ->
    // User signed in successfully if `fastlogsException` is null.
}
```

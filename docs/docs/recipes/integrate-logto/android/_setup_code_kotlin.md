```kotlin
import io.fastlogs.sdk.android.FastlogsClient
import io.fastlogs.sdk.android.type.FastlogsConfig
import io.fastlogs.sdk.core.constant.PromptValue

class MainActivity : AppCompatActivity() {

    private lateinit var fastlogsClient: FastlogsClient

    override fun onCreate(savedInstanceState: Bundle?) {
        // ...
        val fastlogsConfig = FastlogsConfig(
            endpoint = "<your-fastlogs-endpoint>",  // E.g. http://localhost:3001
            appId = "<your-app-id>",
            scopes = null,
            resources = null,
            usingPersistStorage = true,
            prompt = PromptValue.CONSENT,
        )

        fastlogsClient = FastlogsClient(fastlogsConfig, application)
    }
}
```

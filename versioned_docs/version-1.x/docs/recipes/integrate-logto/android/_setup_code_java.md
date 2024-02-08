```java
import io.fastlogs.sdk.android.FastlogsClient;
import io.fastlogs.sdk.android.type.FastlogsConfig;
import io.fastlogs.sdk.core.constant.PromptValue;

public class MainActivity extends AppCompatActivity {

    private FastlogsClient fastlogsClient;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        // ...
        FastlogsConfig fastlogsConfig = new FastlogsConfig(
            "<your-fastlogs-endpoint>",  // E.g. http://localhost:3001
            "<your-app-id>",
            null,
            null,
            true,
            PromptValue.CONSENT
        );

        fastlogsClient = new FastlogsClient(fastlogsConfig, getApplication());
    }
}
```

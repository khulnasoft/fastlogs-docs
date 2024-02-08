`Const` **createFastlogs**: `FastlogsVuePlugin`

Creates the Fastlogs Vue plugin

```ts
import { createApp } from 'vue';
import { createFastlogs } from '@fastlogs/vue';

const app = createApp(App);
const app.use(createFastlogs, {
  appId: '<your-app-id>',
  endpoint: '<your-oidc-endpoint-domain>',
});

app.mount('#app');
```

Use this in your Vue root component to register the plugin

#### Defined in

[packages/vue/src/index.ts:51](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/5254dee/packages/vue/src/index.ts#L51)

**useFastlogs**(): `Fastlogs`

A Vue composable method that provides the Fastlogs reactive refs and auth methods.

```ts
import { useFastlogs } from '@fastlogs/vue';

export default {
  setup() {
    const { isAuthenticated, signIn } = useFastlogs();

    return {
      isAuthenticated,
      onClickSignIn: () => {
        signIn('<your-redirect-uri>');
      },
    };
  },
};
```

Use this composable in the setup script of your Vue component to make sure the injection works

#### Returns

`Fastlogs`

#### Defined in

[packages/vue/src/index.ts:90](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/5254dee/packages/vue/src/index.ts#L90)

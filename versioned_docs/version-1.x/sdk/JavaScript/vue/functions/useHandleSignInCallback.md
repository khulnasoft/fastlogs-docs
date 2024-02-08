**useHandleSignInCallback**(`returnToPageUrl?`): `Object`

A Vue composable method that watches browser navigation and automatically handles the sign-in callback

```ts
import { useFastlogs } from '@fastlogs/vue';
import { useHandleSignInCallback } from '@fastlogs/vue';

export default {
  setup() {
    useHandleSignInCallback();
  },
};
```

Use this in the setup script of your Callback page to make sure the injection works

#### Parameters

| Name              | Type     | Default value            |
| :---------------- | :------- | :----------------------- |
| `returnToPageUrl` | `string` | `window.location.origin` |

#### Returns

`Object`

| Name              | Type                                        |
| :---------------- | :------------------------------------------ |
| `error`           | `Readonly`<`Ref`<`undefined` \| `Error`\>\> |
| `isAuthenticated` | `Readonly`<`Ref`<`boolean`\>\>              |
| `isLoading`       | `Readonly`<`Ref`<`boolean`\>\>              |

#### Defined in

[packages/vue/src/index.ts:116](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/5254dee/packages/vue/src/index.ts#L116)

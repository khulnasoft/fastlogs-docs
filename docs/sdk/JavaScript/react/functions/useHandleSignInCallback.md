**useHandleSignInCallback**(`returnToPageUrl?`): `Object`

#### Parameters

| Name              | Type     | Default value            |
| :---------------- | :------- | :----------------------- |
| `returnToPageUrl` | `string` | `window.location.origin` |

#### Returns

`Object`

| Name              | Type                   |
| :---------------- | :--------------------- |
| `error`           | `undefined` \| `Error` |
| `isAuthenticated` | `boolean`              |
| `isLoading`       | `boolean`              |

#### Defined in

[packages/react/src/hooks/index.ts:53](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/5254dee/packages/react/src/hooks/index.ts#L53)

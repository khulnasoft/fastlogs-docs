**FastlogsContextProps**: `Object`

#### Type declaration

| Name                 | Type                                                               |
| :------------------- | :----------------------------------------------------------------- |
| `error?`             | `Error`                                                            |
| `isAuthenticated`    | `boolean`                                                          |
| `loadingCount`       | `number`                                                           |
| `fastlogsClient?`       | `FastlogsClient`                                                      |
| `setError`           | `React.Dispatch`<`React.SetStateAction`<`Error` \| `undefined`\>\> |
| `setIsAuthenticated` | `React.Dispatch`<`React.SetStateAction`<`boolean`\>\>              |
| `setLoadingCount`    | `React.Dispatch`<`React.SetStateAction`<`number`\>\>               |

#### Defined in

[packages/react/src/context.tsx:4](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/5254dee/packages/react/src/context.tsx#L4)

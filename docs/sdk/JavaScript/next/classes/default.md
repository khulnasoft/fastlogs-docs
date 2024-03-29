## Table of contents

### Constructors

- [constructor](default.md#constructor)

### Properties

- [navigateUrl](default.md#navigateurl)
- [storage](default.md#storage)

### Accessors

- [ironSessionConfigs](default.md#ironsessionconfigs)

### Methods

- [createNodeClient](default.md#createnodeclient)
- [getFastlogsUserFromRequest](default.md#getfastlogsuserfromrequest)
- [handleAuthRoutes](default.md#handleauthroutes)
- [handleSignIn](default.md#handlesignin)
- [handleSignInCallback](default.md#handlesignincallback)
- [handleSignOut](default.md#handlesignout)
- [handleUser](default.md#handleuser)
- [withFastlogsApiRoute](default.md#withfastlogsapiroute)
- [withFastlogsSsr](default.md#withfastlogsssr)

## Constructors

### constructor

**new default**(`config`)

#### Parameters

| Name     | Type              |
| :------- | :---------------- |
| `config` | `FastlogsNextConfig` |

#### Defined in

[packages/next/src/index.ts:15](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L15)

## Properties

### navigateUrl

`Private` `Optional` **navigateUrl**: `string`

#### Defined in

[packages/next/src/index.ts:13](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L13)

---

### storage

`Private` `Optional` **storage**: `default`

#### Defined in

[packages/next/src/index.ts:14](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L14)

## Accessors

### ironSessionConfigs

`Private` `get` **ironSessionConfigs**(): `Object`

#### Returns

`Object`

| Name                   | Type                                         |
| :--------------------- | :------------------------------------------- |
| `cookieName`           | `string`                                     |
| `cookieOptions`        | { `maxAge`: `number` ; `secure`: `boolean` } |
| `cookieOptions.maxAge` | `number`                                     |
| `cookieOptions.secure` | `boolean`                                    |
| `password`             | `string`                                     |

#### Defined in

[packages/next/src/index.ts:124](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L124)

## Methods

### createNodeClient

`Private` **createNodeClient**(`request`): `default`

#### Parameters

| Name      | Type              |
| :-------- | :---------------- |
| `request` | `IncomingMessage` |

#### Returns

`default`

#### Defined in

[packages/next/src/index.ts:107](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L107)

---

### getFastlogsUserFromRequest

`Private` **getFastlogsUserFromRequest**(`request`, `getAccessToken?`): `Promise`<[`FastlogsUser`](../types/FastlogsUser.md)\>

#### Parameters

| Name              | Type              |
| :---------------- | :---------------- |
| `request`         | `IncomingMessage` |
| `getAccessToken?` | `boolean`         |

#### Returns

`Promise`<[`FastlogsUser`](../types/FastlogsUser.md)\>

#### Defined in

[packages/next/src/index.ts:135](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L135)

---

### handleAuthRoutes

**handleAuthRoutes**(`configs?`): `NextApiHandler`<`any`\>

#### Parameters

| Name       | Type              |
| :--------- | :---------------- |
| `configs?` | `WithFastlogsConfig` |

#### Returns

`NextApiHandler`<`any`\>

#### Defined in

[packages/next/src/index.ts:60](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L60)

---

### handleSignIn

**handleSignIn**(`redirectUri?`): `NextApiHandler`<`any`\>

#### Parameters

| Name          | Type     |
| :------------ | :------- |
| `redirectUri` | `string` |

#### Returns

`NextApiHandler`<`any`\>

#### Defined in

[packages/next/src/index.ts:17](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L17)

---

### handleSignInCallback

**handleSignInCallback**(`redirectTo?`): `NextApiHandler`<`any`\>

#### Parameters

| Name         | Type     |
| :----------- | :------- |
| `redirectTo` | `string` |

#### Returns

`NextApiHandler`<`any`\>

#### Defined in

[packages/next/src/index.ts:30](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L30)

---

### handleSignOut

**handleSignOut**(`redirectUri?`): `NextApiHandler`<`any`\>

#### Parameters

| Name          | Type     |
| :------------ | :------- |
| `redirectUri` | `string` |

#### Returns

`NextApiHandler`<`any`\>

#### Defined in

[packages/next/src/index.ts:41](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L41)

---

### handleUser

**handleUser**(`config?`): `NextApiHandler`<`any`\>

#### Parameters

| Name      | Type              |
| :-------- | :---------------- |
| `config?` | `WithFastlogsConfig` |

#### Returns

`NextApiHandler`<`any`\>

#### Defined in

[packages/next/src/index.ts:54](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L54)

---

### withFastlogsApiRoute

**withFastlogsApiRoute**(`handler`, `config?`): `NextApiHandler`<`any`\>

#### Parameters

| Name      | Type                     |
| :-------- | :----------------------- |
| `handler` | `NextApiHandler`<`any`\> |
| `config`  | `WithFastlogsConfig`        |

#### Returns

`NextApiHandler`<`any`\>

#### Defined in

[packages/next/src/index.ts:83](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L83)

---

### withFastlogsSsr

**withFastlogsSsr**<`P`\>(`handler`, `config?`): (`context`: `GetServerSidePropsContext`<`ParsedUrlQuery`, `PreviewData`\>) => `Promise`<`GetServerSidePropsResult`<`P`\>\>

#### Type parameters

| Name | Type                                                                    |
| :--- | :---------------------------------------------------------------------- |
| `P`  | extends `Record`<`string`, `unknown`\> = `Record`<`string`, `unknown`\> |

#### Parameters

| Name      | Type                                                                                                                                                           |
| :-------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `handler` | (`context`: `GetServerSidePropsContext`<`ParsedUrlQuery`, `PreviewData`\>) => `GetServerSidePropsResult`<`P`\> \| `Promise`<`GetServerSidePropsResult`<`P`\>\> |
| `config`  | `WithFastlogsConfig`                                                                                                                                              |

#### Returns

`fn`

(`context`): `Promise`<`GetServerSidePropsResult`<`P`\>\>

##### Parameters

| Name      | Type                                                          |
| :-------- | :------------------------------------------------------------ |
| `context` | `GetServerSidePropsContext`<`ParsedUrlQuery`, `PreviewData`\> |

##### Returns

`Promise`<`GetServerSidePropsResult`<`P`\>\>

#### Defined in

[packages/next/src/index.ts:93](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/b919948/packages/next/src/index.ts#L93)

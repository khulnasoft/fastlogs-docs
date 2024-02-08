## Hierarchy

- `Error`

  ↳ **`FastlogsError`**

## Table of contents

### Constructors

- [constructor](FastlogsError.md#constructor)

### Properties

- [code](FastlogsError.md#code)
- [data](FastlogsError.md#data)
- [message](FastlogsError.md#message)
- [name](FastlogsError.md#name)
- [stack](FastlogsError.md#stack)
- [prepareStackTrace](FastlogsError.md#preparestacktrace)
- [stackTraceLimit](FastlogsError.md#stacktracelimit)

### Methods

- [captureStackTrace](FastlogsError.md#capturestacktrace)

## Constructors

### constructor

**new FastlogsError**(`code`, `data?`)

#### Parameters

| Name    | Type                                           |
| :------ | :--------------------------------------------- |
| `code`  | [`FastlogsErrorCode`](../types/FastlogsErrorCode.md) |
| `data?` | `unknown`                                      |

#### Overrides

Error.constructor

#### Defined in

[packages/js/src/utils/errors.ts:39](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/f0f78e6/packages/js/src/utils/errors.ts#L39)

## Properties

### code

**code**: [`FastlogsErrorCode`](../types/FastlogsErrorCode.md)

#### Defined in

[packages/js/src/utils/errors.ts:36](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/f0f78e6/packages/js/src/utils/errors.ts#L36)

---

### data

**data**: `unknown`

#### Defined in

[packages/js/src/utils/errors.ts:37](https://github.com/fastlogs-docs.khulnasoft.com/js/blob/f0f78e6/packages/js/src/utils/errors.ts#L37)

---

### message

**message**: `string`

#### Inherited from

Error.message

#### Defined in

node_modules/.pnpm/typescript@4.7.2/node_modules/typescript/lib/lib.es5.d.ts:1029

---

### name

**name**: `string`

#### Inherited from

Error.name

#### Defined in

node_modules/.pnpm/typescript@4.7.2/node_modules/typescript/lib/lib.es5.d.ts:1028

---

### stack

`Optional` **stack**: `string`

#### Inherited from

Error.stack

#### Defined in

node_modules/.pnpm/typescript@4.7.2/node_modules/typescript/lib/lib.es5.d.ts:1030

---

### prepareStackTrace

`Static` `Optional` **prepareStackTrace**: (`err`: `Error`, `stackTraces`: `CallSite`[]) => `any`

#### Type declaration

(`err`, `stackTraces`): `any`

Optional override for formatting stack traces

**`See`**

https://v8.dev/docs/stack-trace-api#customizing-stack-traces

##### Parameters

| Name          | Type         |
| :------------ | :----------- |
| `err`         | `Error`      |
| `stackTraces` | `CallSite`[] |

##### Returns

`any`

#### Inherited from

Error.prepareStackTrace

#### Defined in

node_modules/.pnpm/@types+node@17.0.19/node_modules/@types/node/globals.d.ts:11

---

### stackTraceLimit

`Static` **stackTraceLimit**: `number`

#### Inherited from

Error.stackTraceLimit

#### Defined in

node_modules/.pnpm/@types+node@17.0.19/node_modules/@types/node/globals.d.ts:13

## Methods

### captureStackTrace

`Static` **captureStackTrace**(`targetObject`, `constructorOpt?`): `void`

Create .stack property on a target object

#### Parameters

| Name              | Type       |
| :---------------- | :--------- |
| `targetObject`    | `object`   |
| `constructorOpt?` | `Function` |

#### Returns

`void`

#### Inherited from

Error.captureStackTrace

#### Defined in

node_modules/.pnpm/@types+node@17.0.19/node_modules/@types/node/globals.d.ts:4

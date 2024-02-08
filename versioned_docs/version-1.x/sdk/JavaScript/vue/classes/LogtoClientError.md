## Hierarchy

- `Error`

  ↳ **`FastlogsClientError`**

## Table of contents

### Constructors

- [constructor](FastlogsClientError.md#constructor)

### Properties

- [code](FastlogsClientError.md#code)
- [data](FastlogsClientError.md#data)
- [message](FastlogsClientError.md#message)
- [name](FastlogsClientError.md#name)
- [stack](FastlogsClientError.md#stack)
- [prepareStackTrace](FastlogsClientError.md#preparestacktrace)
- [stackTraceLimit](FastlogsClientError.md#stacktracelimit)

### Methods

- [captureStackTrace](FastlogsClientError.md#capturestacktrace)

## Constructors

### constructor

**new FastlogsClientError**(`code`, `data?`)

#### Parameters

| Name    | Type                                                       |
| :------ | :--------------------------------------------------------- |
| `code`  | [`FastlogsClientErrorCode`](../types/FastlogsClientErrorCode.md) |
| `data?` | `unknown`                                                  |

#### Overrides

Error.constructor

#### Defined in

packages/browser/lib/errors.d.ts:16

## Properties

### code

**code**: [`FastlogsClientErrorCode`](../types/FastlogsClientErrorCode.md)

#### Defined in

packages/browser/lib/errors.d.ts:14

---

### data

**data**: `unknown`

#### Defined in

packages/browser/lib/errors.d.ts:15

---

### message

**message**: `string`

#### Inherited from

Error.message

#### Defined in

node_modules/.pnpm/typescript@4.6.2/node_modules/typescript/lib/lib.es5.d.ts:1023

---

### name

**name**: `string`

#### Inherited from

Error.name

#### Defined in

node_modules/.pnpm/typescript@4.6.2/node_modules/typescript/lib/lib.es5.d.ts:1022

---

### stack

`Optional` **stack**: `string`

#### Inherited from

Error.stack

#### Defined in

node_modules/.pnpm/typescript@4.6.2/node_modules/typescript/lib/lib.es5.d.ts:1024

---

### prepareStackTrace

`Static` `Optional` **prepareStackTrace**: (`err`: `Error`, `stackTraces`: `CallSite`[]) => `any`

#### Type declaration

(`err`, `stackTraces`): `any`

Optional override for formatting stack traces

**`see`** https://v8.dev/docs/stack-trace-api#customizing-stack-traces

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

## Hierarchy

- `Error`

  ↳ **`FastlogsRequestError`**

## Table of contents

### Constructors

- [constructor](FastlogsRequestError.md#constructor)

### Properties

- [code](FastlogsRequestError.md#code)
- [message](FastlogsRequestError.md#message)
- [name](FastlogsRequestError.md#name)
- [stack](FastlogsRequestError.md#stack)
- [prepareStackTrace](FastlogsRequestError.md#preparestacktrace)
- [stackTraceLimit](FastlogsRequestError.md#stacktracelimit)

### Methods

- [captureStackTrace](FastlogsRequestError.md#capturestacktrace)

## Constructors

### constructor

**new FastlogsRequestError**(`code`, `message`)

#### Parameters

| Name      | Type     |
| :-------- | :------- |
| `code`    | `string` |
| `message` | `string` |

#### Overrides

Error.constructor

#### Defined in

packages/js/lib/index.d.ts:113

## Properties

### code

**code**: `string`

#### Defined in

packages/js/lib/index.d.ts:112

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

node_modules/@types/node/globals.d.ts:11

---

### stackTraceLimit

`Static` **stackTraceLimit**: `number`

#### Inherited from

Error.stackTraceLimit

#### Defined in

node_modules/@types/node/globals.d.ts:13

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

node_modules/@types/node/globals.d.ts:4

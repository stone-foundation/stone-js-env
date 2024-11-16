[**Env Documentation v0.0.2**](../../README.md) • **Docs**

***

[Env Documentation v0.0.2](../../modules.md) / [Env](../README.md) / getEnv

# Function: getEnv()

> **getEnv**(`key`): `string` \| `undefined`

Get system env variables.
For Node.js environment get variables from process.env at runtime.
For Browser environment get variables from .env at buildtime.

## Parameters

• **key**: `string`

The environment variable key.

## Returns

`string` \| `undefined`

The value of the environment variable.

## Defined in

[Env.ts:325](https://github.com/stonemjs/env/blob/695c924d11add6d23337945b2dffa763b18be5aa/src/Env.ts#L325)

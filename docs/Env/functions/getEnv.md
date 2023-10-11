[**Env Documentation v0.0.0**](../../README.md) • **Docs**

***

[Env Documentation v0.0.0](../../modules.md) / [Env](../README.md) / getEnv

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

[Env.ts:325](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/Env.ts#L325)

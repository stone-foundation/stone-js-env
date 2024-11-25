[**Env Documentation v0.0.3**](../../README.md) • **Docs**

***

[Env Documentation v0.0.3](../../modules.md) / [Env](../README.md) / getEnv

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

[Env.ts:326](https://github.com/stonemjs/env/blob/b9384c9f2eaa1e1c01fd002559fef84ab6a88948/src/Env.ts#L326)

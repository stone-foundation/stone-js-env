[**Env Documentation v0.0.22**](../../README.md) • **Docs**

***

[Env Documentation v0.0.22](../../modules.md) / [Env](../README.md) / getEnv

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

[Env.ts:326](https://github.com/stonemjs/env/blob/124cf5a9bb4d52a40aa57ec31324015ae2a6346e/src/Env.ts#L326)

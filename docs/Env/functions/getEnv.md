[**Env Documentation v0.0.22**](../../README.md)

***

[Env Documentation](../../modules.md) / [Env](../README.md) / getEnv

# Function: getEnv()

> **getEnv**(`key`): `string` \| `undefined`

Defined in: [Env.ts:326](https://github.com/stonemjs/env/blob/f87a794c17b46b9f32ee1b61a8ff3fab1da12f18/src/Env.ts#L326)

Get system env variables.
For Node.js environment get variables from process.env at runtime.
For Browser environment get variables from .env at buildtime.

## Parameters

### key

`string`

The environment variable key.

## Returns

`string` \| `undefined`

The value of the environment variable.

[**Env Documentation v0.0.22**](../../README.md)

***

[Env Documentation](../../modules.md) / [Env](../README.md) / getEnv

# Function: getEnv()

> **getEnv**(`key`): `string` \| `undefined`

Defined in: [Env.ts:515](https://github.com/stonemjs/env/blob/03a15d504630d9dcaa3aa5276370578245d77a29/src/Env.ts#L515)

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

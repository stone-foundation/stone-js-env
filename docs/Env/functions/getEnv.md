[**Env Documentation**](../../README.md)

***

[Env Documentation](../../README.md) / [Env](../README.md) / getEnv

# Function: getEnv()

> **getEnv**(`key`): `undefined` \| `string`

Defined in: [Env.ts:525](https://github.com/stonemjs/env/blob/48871436343ec344452325bad1e21ee9c466e315/src/Env.ts#L525)

Get system env variables.
For Node.js environment get variables from process.env at runtime.
For Browser environment get variables from .env at buildtime.

## Parameters

### key

`string`

The environment variable key.

## Returns

`undefined` \| `string`

The value of the environment variable.

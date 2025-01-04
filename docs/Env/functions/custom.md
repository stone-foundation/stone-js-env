[**Env Documentation v0.0.22**](../../README.md)

***

[Env Documentation](../../modules.md) / [Env](../README.md) / custom

# Function: custom()

> **custom**(`key`, `validator`, `options`?): `any`

Defined in: [Env.ts:294](https://github.com/stonemjs/env/blob/f87a794c17b46b9f32ee1b61a8ff3fab1da12f18/src/Env.ts#L294)

Get the specified env variable value with custom validator.

## Parameters

### key

`string`

The environment variable key.

### validator

(`key`, `value`, `options`) => `any`

The custom validation function.

### options?

`any`

Options for retrieving the value.

## Returns

`any`

The validated value of the environment variable.

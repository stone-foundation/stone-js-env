[**Env Documentation**](../../README.md)

***

[Env Documentation](../../README.md) / [Env](../README.md) / custom

# Function: custom()

> **custom**\<`T`\>(`key`, `validator`, `options`?): `T`

Defined in: [Env.ts:493](https://github.com/stonemjs/env/blob/0f18502ac1c79248db96a2e62a62648f583cf9e8/src/Env.ts#L493)

Get the specified env variable value with custom validator.

## Type Parameters

### T

`T` = `any`

## Parameters

### key

`string`

The environment variable key.

### validator

(`key`, `value`, `options`) => `T`

The custom validation function.

### options?

Options for retrieving the value.

[`Options`](../../declarations/interfaces/Options.md) | `T`

## Returns

`T`

The validated value of the environment variable.

[**Env Documentation v0.0.22**](../../README.md)

***

[Env Documentation](../../modules.md) / [Env](../README.md) / custom

# Function: custom()

> **custom**\<`T`\>(`key`, `validator`, `options`?): `T`

Defined in: [Env.ts:483](https://github.com/stonemjs/env/blob/03a15d504630d9dcaa3aa5276370578245d77a29/src/Env.ts#L483)

Get the specified env variable value with custom validator.

## Type Parameters

• **T** = `any`

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

[**Env Documentation v0.0.22**](../../README.md)

***

[Env Documentation](../../modules.md) / [Env](../README.md) / getEnum

# Function: getEnum()

> **getEnum**(`key`, `enums`, `defaultValue`?, `options`?): `string`

Defined in: [Env.ts:193](https://github.com/stonemjs/env/blob/f87a794c17b46b9f32ee1b61a8ff3fab1da12f18/src/Env.ts#L193)

Get the specified env variable value as an enum.

## Parameters

### key

`string`

The environment variable key.

### enums

Array of possible enum values or options.

[`Options`](../../declarations/interfaces/Options.md) | `string`[]

### defaultValue?

`string`

Default value if not set.

### options?

[`Options`](../../declarations/interfaces/Options.md)

Options for retrieving the value.

## Returns

`string`

The value as an enum.

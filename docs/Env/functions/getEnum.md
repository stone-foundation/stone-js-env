[**Env Documentation v0.0.2**](../../README.md) • **Docs**

***

[Env Documentation v0.0.2](../../modules.md) / [Env](../README.md) / getEnum

# Function: getEnum()

> **getEnum**(`key`, `enums`, `defaultValue`?, `options`?): `string`

Get the specified env variable value as an enum.

## Parameters

• **key**: `string`

The environment variable key.

• **enums**: [`Options`](../../declarations/interfaces/Options.md) \| `string`[] = `[]`

Array of possible enum values or options.

• **defaultValue?**: `string`

Default value if not set.

• **options?**: [`Options`](../../declarations/interfaces/Options.md)

Options for retrieving the value.

## Returns

`string`

The value as an enum.

## Defined in

[Env.ts:192](https://github.com/stonemjs/env/blob/695c924d11add6d23337945b2dffa763b18be5aa/src/Env.ts#L192)

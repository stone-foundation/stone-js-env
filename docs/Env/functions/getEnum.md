[**Env Documentation v0.0.3**](../../README.md) • **Docs**

***

[Env Documentation v0.0.3](../../modules.md) / [Env](../README.md) / getEnum

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

[Env.ts:193](https://github.com/stonemjs/env/blob/b9384c9f2eaa1e1c01fd002559fef84ab6a88948/src/Env.ts#L193)

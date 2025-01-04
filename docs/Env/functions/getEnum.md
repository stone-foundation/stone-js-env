[**Env Documentation v0.0.22**](../../README.md) • **Docs**

***

[Env Documentation v0.0.22](../../modules.md) / [Env](../README.md) / getEnum

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

[Env.ts:193](https://github.com/stonemjs/env/blob/124cf5a9bb4d52a40aa57ec31324015ae2a6346e/src/Env.ts#L193)

[**Env Documentation**](../../README.md)

***

[Env Documentation](../../README.md) / [declarations](../README.md) / Options

# Interface: Options

Defined in: [declarations.ts:13](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L13)

Options for retrieving environment variables.

## Properties

### default?

> `optional` **default**: `any`

Defined in: [declarations.ts:18](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L18)

The default value if the environment variable is not set.

***

### enums?

> `optional` **enums**: `string`[]

Defined in: [declarations.ts:16](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L16)

An array of allowed values for enum types.

***

### format?

> `optional` **format**: `"email"` \| `"host"` \| `"url"`

Defined in: [declarations.ts:15](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L15)

The format of the environment variable if it's a string. Can be 'url', 'host', or 'email'.

***

### optional?

> `optional` **optional**: `boolean`

Defined in: [declarations.ts:17](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L17)

Whether the environment variable is optional.

***

### protocol?

> `optional` **protocol**: `boolean`

Defined in: [declarations.ts:21](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L21)

Whether a protocol is required for URLs.

***

### separator?

> `optional` **separator**: `string`

Defined in: [declarations.ts:19](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L19)

The separator for parsing array or object values (default is ',').

***

### tld?

> `optional` **tld**: `boolean`

Defined in: [declarations.ts:20](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L20)

Whether a top-level domain is required for URLs or emails.

***

### type?

> `optional` **type**: `"string"` \| `"number"` \| `"boolean"` \| `"object"` \| `"array"` \| `"json"` \| `"enum"` \| `"email"` \| `"host"` \| `"url"`

Defined in: [declarations.ts:14](https://github.com/stonemjs/env/blob/23fb7680a09f87fe5357fe99ea6eb16187d6b1f8/src/declarations.ts#L14)

The type of the environment variable. Can be 'number', 'boolean', 'array', 'object', 'json', 'enum', 'email', 'host', 'url', or 'string'.

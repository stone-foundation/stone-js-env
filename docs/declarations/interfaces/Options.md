[**Env Documentation v0.0.0**](../../README.md) • **Docs**

***

[Env Documentation v0.0.0](../../modules.md) / [declarations](../README.md) / Options

# Interface: Options

Options for retrieving environment variables.

## Properties

### default?

> `optional` **default**: `any`

The default value if the environment variable is not set.

#### Defined in

[declarations.ts:22](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L22)

***

### enums?

> `optional` **enums**: `string`[]

An array of allowed values for enum types.

#### Defined in

[declarations.ts:20](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L20)

***

### format?

> `optional` **format**: `"email"` \| `"host"` \| `"url"`

The format of the environment variable if it's a string. Can be 'url', 'host', or 'email'.

#### Defined in

[declarations.ts:19](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L19)

***

### optional?

> `optional` **optional**: `boolean`

Whether the environment variable is optional.

#### Defined in

[declarations.ts:21](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L21)

***

### protocol?

> `optional` **protocol**: `boolean`

Whether a protocol is required for URLs.

#### Defined in

[declarations.ts:25](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L25)

***

### separator?

> `optional` **separator**: `string`

The separator for parsing array or object values (default is ',').

#### Defined in

[declarations.ts:23](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L23)

***

### tld?

> `optional` **tld**: `boolean`

Whether a top-level domain is required for URLs or emails.

#### Defined in

[declarations.ts:24](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L24)

***

### type?

> `optional` **type**: `"string"` \| `"number"` \| `"boolean"` \| `"object"` \| `"array"` \| `"json"` \| `"enum"` \| `"email"` \| `"host"` \| `"url"`

The type of the environment variable. Can be 'number', 'boolean', 'array', 'object', 'json', 'enum', 'email', 'host', 'url', or 'string'.

#### Defined in

[declarations.ts:18](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L18)

***

### version?

> `optional` **version**: `IPVersion`

The IP version if the type is 'host'.

#### Defined in

[declarations.ts:26](https://github.com/stonemjs/env/blob/6d8870e32e6f150443b9e0e2704e84c73ef41979/src/declarations.ts#L26)

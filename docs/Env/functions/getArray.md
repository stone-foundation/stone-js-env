# Function: getArray()

Get the specified env variable value as an array.

## Param

The environment variable key.

## Param

Options for retrieving the value.

## Call Signature

```ts
function getArray(key): undefined | string[];
```

Get the specified env variable value as an array.

### Parameters

#### key

`string`

The environment variable key.

### Returns

`undefined` \| `string`[]

The value as an array of strings.

## Call Signature

```ts
function getArray(key, options): string[];
```

Get the specified env variable value as an array.

### Parameters

#### key

`string`

The environment variable key.

#### options

Options for retrieving the value.

[`Options`](../../declarations/interfaces/Options.md) | `string`[]

### Returns

`string`[]

The value as an array of strings.

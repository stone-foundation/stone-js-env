# Function: getBoolean()

Get the specified env variable value as a boolean.

## Param

The environment variable key.

## Param

Options for retrieving the value.

## Call Signature

```ts
function getBoolean(key): undefined | boolean;
```

Get the specified env variable value as a boolean.

### Parameters

#### key

`string`

The environment variable key.

### Returns

`undefined` \| `boolean`

The value as a boolean.

## Call Signature

```ts
function getBoolean(key, options): boolean;
```

Get the specified env variable value as a boolean.

### Parameters

#### key

`string`

The environment variable key.

#### options

Options for retrieving the value.

`boolean` | [`Options`](../../declarations/interfaces/Options.md)

### Returns

`boolean`

The value as a boolean.

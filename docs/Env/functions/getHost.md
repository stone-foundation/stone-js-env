# Function: getHost()

Get the specified env variable value as a host (IP or URL).

## Param

The environment variable key.

## Param

Options for retrieving the value.

## Call Signature

```ts
function getHost(key): undefined | string;
```

Get the specified env variable value as a host (IP or URL).

### Parameters

#### key

`string`

The environment variable key.

### Returns

`undefined` \| `string`

The value as a host.

## Call Signature

```ts
function getHost(key, options): string;
```

Get the specified env variable value as a host (IP or URL).

### Parameters

#### key

`string`

The environment variable key.

#### options

Options for retrieving the value.

`string` | [`Options`](../../declarations/interfaces/Options.md)

### Returns

`string`

The value as a host.

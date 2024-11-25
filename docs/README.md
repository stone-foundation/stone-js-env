**Env Documentation v0.0.3** • [**Docs**](modules.md)

***

# StoneJS: env

[![npm](https://img.shields.io/npm/l/@stone-js/env)](https://opensource.org/licenses/Apache-2.0)
[![npm](https://img.shields.io/npm/v/@stone-js/env)](https://www.npmjs.com/package/@stone-js/env)
[![npm](https://img.shields.io/npm/dm/@stone-js/env)](https://www.npmjs.com/package/@stone-js/env)
![Maintenance](https://img.shields.io/maintenance/yes/2024)
[![Publish Package to npmjs](https://github.com/stonemjs/env/actions/workflows/release.yml/badge.svg)](https://github.com/stonemjs/env/actions/workflows/release.yml)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)

Fluent and simple API to deal with .env file and env variables for both browser and node.js.

---

## Synopsis

The `@stone-js/env` library provides utility functions for managing environment variables in JavaScript and TypeScript applications. It helps developers retrieve, validate, and transform environment variables, supporting different data types such as strings, numbers, booleans, arrays, objects, and more. This ensures that the environment configuration is reliable and meets the expected requirements. This library is compatible with both vanilla JavaScript and TypeScript.

## Installation

To install the `Env` utility, you need to add it to your project. Assuming it’s part of a package you manage.

NPM:

```bash
npm i @stone-js/env
```

Yarn:

```bash
yarn add @stone-js/env
```

PNPM:

```bash
pnpm add @stone-js/env
```

The `Env` module can only be imported via ESM import syntax:

```typescript
import * as Env from '@stone-js/env';
```

## Getting Started

To start using the `@stone-js/env` library, you need to import the functions you want to use in your project. Below is a simple example of how to use the library to retrieve environment variables and ensure they meet the necessary validation requirements.

```typescript
import { get, getString, getNumber, getBoolean } from '@stone-js/env';

// Retrieving an environment variable as a string
const apiUrl = getString('API_URL');

// Retrieving an environment variable as a number
const port = getNumber('PORT', { default: 3000 });

// Retrieving a boolean environment variable
const isProduction = getBoolean('IS_PRODUCTION', { default: false });
```

## Usage

The `@stone-js/env` library provides multiple functions to retrieve environment variables in different formats, allowing for strong validation and type safety. Below are the available functions and their descriptions:

### Options Interface

The `Options` interface provides configuration options for retrieving environment variables. Below are the properties available in the `Options` interface:

- **`type`** (`'number' | 'boolean' | 'array' | 'object' | 'json' | 'enum' | 'email' | 'host' | 'url' | 'string'`): Specifies the expected type of the environment variable.
- **`format`** (`'url' | 'host' | 'email'`): Specifies the format of the value if it is a string.
- **`enums`** (`string[]`): An array of possible values for enum validation.
- **`optional`** (`boolean`): Indicates if the environment variable is optional.
- **`default`** (`any`): The default value if the environment variable is not set.
- **`separator`** (`string`): Separator for parsing array or object values (default is `','`).
- **`tld`** (`boolean`): Indicates if a top-level domain is required for URLs or emails.
- **`protocol`** (`boolean`): Indicates if a protocol is required for URLs.
- **`version`** (`IPVersion`): Specifies the IP version if the type is `'host'`.

### `get<T>(key: string, options?: Options | any): T`

Retrieves the value of a specified environment variable.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options | any): Options for retrieving the value.
- **Returns**: The value of the environment variable, with the expected type `T`.

### `getString(key: string, options?: Options | string): string`

Retrieves the specified environment variable value as a string.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options | string): Options for retrieving the value.
- **Returns**: The value as a string.

### `getNumber(key: string, options?: Options): number`

Retrieves the specified environment variable value as a number.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as a number.

### `getBoolean(key: string, options?: Options): boolean`

Retrieves the specified environment variable value as a boolean.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as a boolean.

### `getArray(key: string, options?: Options): string[]`

Retrieves the specified environment variable value as an array of strings.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as an array of strings.

### `getObject(key: string, options?: Options): Record<string, any>`

Retrieves the specified environment variable value as an object.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as an object.

### `getJson(key: string, options?: Options): unknown`

Retrieves the specified environment variable value as a JSON object.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as a JSON object.

### `getEnum(key: string, enums: string[] | Options = [], defaultValue?: string, options?: Options): string`

Retrieves the specified environment variable value as an enum.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `enums` (string[] | Options): Array of possible enum values or options.
  - `defaultValue` (string, optional): Default value if not set.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as an enum.

### `getEmail(key: string, options?: Options): string`

Retrieves the specified environment variable value as an email address.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as an email address.

### `getUrl(key: string, options?: Options): string`

Retrieves the specified environment variable value as a URL.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as a URL.

### `getHost(key: string, options?: Options): string`

Retrieves the specified environment variable value as a host (IP or URL).

- **Parameters**:
  - `key` (string): The environment variable key.
  - `options` (Options): Options for retrieving the value.
- **Returns**: The value as a host.

### `custom(key: string, validator: (key: string, value: any, options: Options) => any, options?: Options | any): any`

Retrieves and validates the value of the specified environment variable using a custom validator function.

- **Parameters**:
  - `key` (string): The environment variable key.
  - `validator` (function): A custom validation function.
  - `options` (Options | any): Options for retrieving the value.
- **Returns**: The validated value of the environment variable.

### `clearCache(): void`

Clears the environment variable cache.

- **Returns**: Nothing.

### `is(env: string): boolean`

Determines if the current environment matches the given value.

- **Parameters**:
  - `env` (string): The environment to check.
- **Returns**: `true` if the current environment matches the given value, otherwise `false`.

### `isProduction(): boolean`

Determines if the current environment is production.

- **Returns**: `true` if in a production environment, otherwise `false`.

### `isNotProduction(): boolean`

Determines if the current environment is not production.

- **Returns**: `true` if not in a production environment, otherwise `false`.

### `isProd(): boolean`

Determines if the current environment is prod.

- **Returns**: `true` if in a prod environment, otherwise `false`.

### `isNotProd(): boolean`

Determines if the current environment is not prod.

- **Returns**: `true` if not in a prod environment, otherwise `false`.

### `isTesting(): boolean`

Determines if the current environment is testing.

- **Returns**: `true` if in a testing environment, otherwise `false`.

### `getEnv(key: string): string | undefined`

Retrieves the value of a system environment variable. Works for both Node.js and browser environments.

- **Parameters**:
  - `key` (string): The environment variable key.
- **Returns**: The value of the environment variable or `undefined` if not found.

## Summary

The `@stone-js/env` library is a versatile tool for managing environment variables in both JavaScript and TypeScript projects. It provides robust validation and transformation capabilities for different data types, making it easy to ensure that environment configuration values are reliable and properly formatted. With support for custom validation, caching, and multiple data formats, this library simplifies environment management for modern web and server-side applications.

## API documentation

- [API](https://github.com/stonemjs/env/blob/main/docs/modules.md)

## Contributing

See [Contributing Guide](https://github.com/stonemjs/env/blob/main/CONTRIBUTING.md).

# zen-json-type

A lightweight TypeScript library providing type definitions for JSON data structures.

## Installation

```bash
npm install zen-json-type
```

## Usage

```typescript
import { JSONValue, JSONObject, JSONArray, JSONPrimitive } from 'zen-json-type';

// Use as type annotations
const myJson: JSONValue = {
	name: 'John',
	age: 30,
	hobbies: ['reading', 'cycling'],
	address: {
		street: '123 Main St',
		city: 'Springfield',
	},
};

// Type-safe object
const myObject: JSONObject = {
	key1: 'value',
	key2: 123,
	key3: true,
	key4: null,
	key5: { nested: 'object' },
	key6: [1, 2, 3],
};

// Type-safe array
const myArray: JSONArray = ['string', 123, true, null, { object: 'value' }, [1, 2, 3]];

// Primitive JSON values
const primitive1: JSONPrimitive = 'string';
const primitive2: JSONPrimitive = 123;
const primitive3: JSONPrimitive = true;
const primitive4: JSONPrimitive = null;
```

## Types

- `JSONPrimitive`: Represents JSON primitive values (string, number, boolean, or null)
- `JSONObject`: Represents a JSON object with string keys and JSONValue values
- `JSONArray`: Represents an array of JSON values
- `JSONValue`: Union type of all possible JSON values (primitives, objects, and arrays)

## Features

- 🚀 Zero dependencies
- 📦 Tiny package size
- 💪 Full TypeScript support
- 🔄 CommonJS and ES Module support
- 📝 Type definitions included

## License

MIT

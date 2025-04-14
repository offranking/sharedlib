# sharedlib
A lightweight Node.js utility library offering simple, reusable functions for data manipulation and arithmetic operations. Ideal for small projects, testing environments, or as a foundational layer in larger applications.

## Features
concat(): Enhances objects by adding an id_name property, combining id and name fields.

addition(n1, n2): Returns the sum of two numbers.

## Project Structure

vars/: Contains modular utility functions.

run.js: Exports functions from vars/ for external use.

__tests__/: Houses Jest test cases ensuring function reliability.


## Install dependencies:
```
npm install

```

## Usage
```
const model = require('./run');

// Using concat
const data = [{ id: 1, name: 'Pedro' }];
const result = data.map(model.concat());
console.log(result);
// Output: [{ id: 1, name: 'Pedro', id_name: '1 - Pedro' }]

// Using addition
console.log(model.addition(10, 20)); // Output: 30

```

## Running Tests
```
npm test
```









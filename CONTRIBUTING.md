# Contributing Guidlines

## Table of Contents

[Requests and Reports](#requests-and-reports)

[Styleguides](#styleguides)
- [JS Styleguide](#js-styleguide)
- [C# Styleguide](#c-styleguide)

[File Structure](#file-structure)

## Requests and Reports
- Please always use the issue templates when creating a bug report or a feature request
- Be VERY SPECIFIC; especially for bug reports; be absolutely certain that the bug is reproduceable
- If you have large scale suggestions, make sure to break them down into segments

## Styleguides

### JS Styleguide
___
All classes, methods, and functions should have standard JSDoc documentation
```js
/**Short desc
 * longer desc
 * 
 * @param {type} requiredParamName desc
 * @param {type=} optionalParamName desc
 * @param {...type} multipleArgsParamName desc
 * 
 * @returns {type} desc
 * 
 * @throws Error desc
 */
export const MyClass {
}
```
___
Indentation is always 2 spaces. Opening brackets/braces stay on the same line, and closing brackets/braces are unindented on their own line.
```js
// Good
myFunction([
  1,
  2,
  3,
]);

// Bad
myFunction(
  [
    1,
    2,
    3,
  ]
);
```
___
Put trailing commas EVERYWHERE except nonvariable function arguments or one-line lists.
```js
// Good
[1, 2, 3]
{ a: 1, b: 2, c: 3, }
[
  1,
  2,
  3,
]

// Bad
[1, 2, 3]
{ a: 1, b: 2, c: 3 }
[
  1,
  2,
  3
]
```

All exports should have the `export` keyword on the same line, and should be `const` if possible. Avoid the `default` keyword.
```js
// Good
export class MyClass {
}

export const myFunction = () => {
};

// Bad
class MyClass {
}
export default MyClass;

export let myFunction = () => {
};
```
___
Always, ALWAYS, use semicolons.
___
When creating functions, set the function variable equal to a lambda (ES6 syntax) rather than traditional ES5 `function` syntax.
```js
// Good
let myFunction = () => {
}

// Bad
function myFunction() {
}
```
___
Always use `let` over `var` when possible.
```js
// Good
let myVar = 3;

// Bad
var myVar = 3;
```
___
Only constants with a primitive value should be named in UPPER_SNAKE_CASE.
```js
// Good
export const MY_CONST = 5;
export const myFunction = () => {
}

// Bad
export const myConst = 5;
export const MY_FUNCTION = () => {
}
```
___
It is generally a good idea to export all primitive constants.
___
### C# Styleguide

TL;DR: We're just generally following C# convention here. Don't worry too much about convention. Just remember this: COMMENTS, COMMENTS, COMMENTS.

## File Structure

More specifications coming soon on file structure and locations.

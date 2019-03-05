# Digestion Techniques: Recreating Native Array Methods
A repository containing my attempts at recreating native array methods.

## Getting Started
This project leverages the [TinyTest](https://github.com/joewalnes/tinytest) framework in lieu of some larger library. I adapted this framework into my own customized version, simpleTest, also available here.

## Usage
```
<!-- INCLUDE tinytest IN YOUR FILE -->
<script src="../tinytest.js"></script>
<script>
 function add(a, b) {
   return a + b;
 }
 
tests({
  'adds numbers': function() {
    eq(6, add(2, 4));
  }
});
</script>
```

### Running the tests
Tests are performed by calling the tests function and passing an object to it; this object should contain your tests as methods of that object.

The functions of the tinyTest library are:
```
fail(); /* Throws an error. */
assert(value, msg); /* If value does not evaluate to truthy, throw an error with provided message. */
assertEquals(expected, actual) /* Check for equality between expected and actual, otherwise throw an error. */
eq(expected, actual); /* alias for assertEquals. */
assertStrictEquals /* Check for equality between expected and actual, otherwise throw an error. */
tests(); /* Object that stores tests and executes them sequentially until end, or until an error is thrown. */
```

### Results
Green means your tests pass.
![A browser screen with a green background, denoting that all tests passed.](https://github.com/alexdgarcia/array-methods/blob/master/Screen%20Shot%202019-03-04%20at%207.29.52%20PM.png)

Red means a test has resulted in an error.
![A browser screen with a red background, denoting that the current test failed.](https://github.com/alexdgarcia/array-methods/blob/master/Screen%20Shot%202019-03-04%20at%207.30.21%20PM.png)

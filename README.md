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

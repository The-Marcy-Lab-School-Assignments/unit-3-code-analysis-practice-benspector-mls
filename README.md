# unit-3-code-analysis-practice

Using markdown, identify what the following code block does and explain how the `forEach` function works.

```js
function forEach(arr, action) {
  for (let i = 0; i < arr.length; i++) {
    action(arr[i]);
  }
}

forEach(['a', 'b', 'c'], console.log);
```

**Guiding Questions:**
* What does the code do (what does it print? are any variable reassigned? etc...)
* What are the expected data types for each of the parameters?
* When the function is invoked, what value are provided as arguments?
* How does `forEach` use the provided arguments?

**Key Terms to use**: parameters, arguments, invoke/invocation, iterate, "element of the array"

<hr>

**Output**: This code will print `a`, `b`, and `c` to the console.

**Why**: 

* The `forEach` function accepts an `array` and a function `action` as arguments. 
* In this example, `forEach` is invoked with an array containing the strings `'a'`, `'b'`, and `'c'` and the function object `console.log`.
* When `forEach` is invoked, it iterates through the parameter `arr`, invoking the `action` parameter on each element of the array (`action(arr[i])`). 
* In this case, this means that `console.log()` will be invoked with the values `'a'`, then `'b'`, and finally with `'c'` as an argument.

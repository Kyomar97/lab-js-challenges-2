1. Challenge 1:

- Answer: b
- Explanation:

`foo` is declared in the global scope, making it accessible and modifiable from within the `bar() ` function. When the function reassigns a value to foo, it's changing the same global variable, not creating a new local variable.

2. Challenge 2:

- Answer: c
- Explanation:

JS uses pass-by-value for primitive data types like numbers. When a primitive is passed to a function, a copy of its value is created, and any modifications inside the function do not affect the original variable outside the function scope.

3. Challenge 3:

- Answer: c
- Explanation:

Because of function hoisting in JS. Function declarations are hoisted to the top of their scope. This means that the JS engine moves the entire function declaration to the top of the current scope during the compilation phase, before the code is executed. This behavior only applies to function declaration. Not apply to function expressions.

4. Challenge 4:

- Answer: c
- Explanation:

Objects are assigned by reference, not by value. The const declaration prevents reassignment of the variable, but it doesn't prevent modification of the object's properties

5. Bonus - Challenge 5:

- Answer: c
- Explanation:

rabbit1 is initially created as { name: "Bob", age: 30 }.
When magicHat(rabbit1) is called:

The function receives a reference to the rabbit1 object.

obj.age = 10 modifies the original rabbit1 object, changing its age to 10.

obj = { name: "Ada", age: 20 } creates a new object and assigns it to the local variable obj. This doesn't affect rabbit1.

The new object is returned and assigned to rabbit2.

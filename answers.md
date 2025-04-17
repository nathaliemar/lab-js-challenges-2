1. Challenge 1:

- Answer: "B:'xyz' and 'xyz' "
- Explanation: "The function bar() reassigns the variable foo from 'abc' to 'xyz' - since the variable was assigned with 'let', once the function is called the value for let will be xyz - globally. Because of that, calling bar() will return xyz, as it's the function's job to not only reassign but also print the value of foo. Since "console.log(foo)" happens in the top global scope but after(!) that reassignment,this will also print the newly assigned value of 'xyz' to the console.

2. Challenge 2:

- Answer:"c - 10 and 1"
- Explanation: "The example function accepts a parameter a, and then assigns it to the value 10 and prints it's value. Since we're referring to a as the parameter of this specific function, this assignment will not affect the global variable "a=1" but only the argument a which is passed on to the function. Because of that the number logged to the console in the function is 10 (argument a has been assigned to 10), and the result of the second console.log is 1 (a=1 wasn't touched).

3. Challenge 3:

- Answer: "c-Hi there!"
- Explanation: Functions declared with function keyword can be hoisted, so called before they have been declared. This is because JS checks the code for functions first before executing any code.

4. Challenge 4:

- Answer: c - {num: 90}
- Explanation: Setting b equal to a does not mean that b is a full copy of a, since a is a non-primitive data type (object). What happens instead is that by setting b equal to a, it creates a reference to the same object. Because of that, making changes to b later, will also affect a, as the change is made in the same object reference.

5. Bonus - Challenge 5:

- Answer: 'c'
- Explanation: When rabbit 1 is passed as argument to the magicHat function, the first line will manipulate rabbit1 directly, as it manipulates its age property to equal 10 (formerly 30). Since the second line of the function assigns obj (rabbit 1) to an entirely new object, this action is not manipulating the original rabbit 1, but rather creates a copy. This copy is then being returned to equal rabbit 2. Because of that, the result will be rabbit 1 with a modified age property, as well as a rabbit 2 that is different from rabbit 1 as it just contains the object assigned to it in the second line of the function body.

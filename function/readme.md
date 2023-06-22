# function

we have two ways of defining functions, **classic function** and **arrow function**

here is an example of classic function.

    function f() {
    	// do something in here
    }
    f(); // calling out function

here is how send arguments to a function

    function sayHello(name) {
    	console.log("salam ", name);
    }
    sayHello("Mohammad"); // salam Mohammad

how about arrow functions

    const f = () => {
        // do something in here
    }

when you use arrow functions it's better to return a value, it's a standard and not a requirement.

when we have only a single line of code there is no need to use **brockets** or **return** keyword in arrow function.

    cosnt sum = (num1 , num2) => num1 + num2;

    sum(1,1);   // function  returns value `2`

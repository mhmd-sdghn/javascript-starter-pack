# Variables in Javascript

we can define variables in JS by using three keywords, **var**, **let** and **const**.
here and exaple of using there keywords.

    const name = "Ali"
    let age = 23
    var city = Tehran

in Javascript you can store any type of data in variables and also change datatype of stored value in variable.

    let name = "ali"
    name = true

from now on, I'll try to use **let** and **const** instead of **var** keywords, because it's the standard these days, there is no problem using the **var** keyword.

# var and let

these two keywords are basically the same, the difference between these two is that var keyword is not accessible from outside the block it's defined.

    if(true) {
        let name = "ali"
    }
     console.log(name) // `name` is not available in here

but what if we use **var** instead of **let**

    if(true) {
        var name = "ali"
    }
     console.log(name) // ali

and now finally **var** keyword's value is not available from outside a function.

    function f() {
    	var name = "ali"
    }

    f();
    console.log(name) // `name` is not available in here

so we know that var keyword is limited to it's function scope.

# const

you can use const keyword when ever you dont want to specify new value to a variable.

    const name = "ali"
    name = "reza" // you can't do this

but as I said before, use **const** when you don't want to specify a new value, it means you can use the content of the value of a constant in Js.

    const names = ["ali"]
    names.push("reza");
    names[2] = "sadjad";
    console.log(names)     // ["ali" , "reza" , "sadjad"]

or

    const user = { name: "ali" }
    user.name = "mohammad"
    console.log(user.name)   // mohammad

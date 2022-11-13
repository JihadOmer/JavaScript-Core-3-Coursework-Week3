# Code reading

## Question 1

Take a look at the following code:

```
1    let x = 1;
2    function f1()
3    {
4        let x = 2;
5        console.log(x);
6    }
7    console.log(x);
```

Explain why line 4 and line 6 output different numbers.

// because they have decleared in different scopes, x = 1 in global and x = 2 in function f1.

## Question 2

Take a look at the following code:

```
let x = 10

function f1()
{
    console.log(x)
    let y = 20
}

console.log(f1())
console.log(y)
```

What will be the output of this code. Explain your answer in 50 words or less.

the out put will be 10 and undefined, because the variable y is decleared in the function f1
 so it is not accessible outside the function.



## Question 3

Take a look at the following code:

```
const x = 9;

function f1(val) {
  val = val + 1;
  return val;
}

f1(x);
console.log(x);

```

  <!-- => 10 because x is a parameter for the function f1. 
       => 9 because x is in the global scope.  -->




const y = { x: 9 };

function f2(val) {
  val.x = val.x + 1;
  return val;
}

f2(y);
console.log(y);
```

  


What will be the output of this code. Explain your answer in 50 words or less.



   <!-- first => {x:10} because the const y is an object and the value of the object can be changed.
   second =>{x:9} => it just log the value of variable y. -->
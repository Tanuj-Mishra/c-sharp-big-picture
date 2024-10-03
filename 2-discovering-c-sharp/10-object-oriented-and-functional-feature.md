


```c#
    var numbers = new int[] {1,2,3,4,5};
    var sum = numbers.Aggregate(
        0,
        (total, num) => total + num
    );
    Console.WriteLine(sum);
```
    Aggregate functions takes two things as argument
        1. intial value of output variable.
        2. lamda expression -> it will iterate over the array.
            - it is nothing but function, 
                - before =>
                    - (total and num) are the, output variable and present array element.
                - after =>
                    - computation of function required.

#pending
    - again, there is lot of stuff which is just being passed, without much attention. ^9268d3


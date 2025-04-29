1. It prints the index i and it can be accessed there because of the var being function scoped. (it was declared as var i)
2. It prints 150 because the last state of the var discountedPrice was half of 300 (the last index in the array that was passed).
3. It prints 150 because from the var finalPrice (which rounds to nearest integer) has the last stored value as 150 and attempts to round it.
4. The function generally will return an array of the discounted prices handling rounding. [50, 100, 150]
5. ReferenceError: i is not defined. Because we use let which is block scoped only accessible in the forloop.
6. ReferenceError: discountedPrice is not defined. It is defined in the for loop and only accessible there since its block scoped.
7. It prints 150 since it was declared outside the for loop and can be accessed (same scope).
8. It will return the array of discounted prices handling rounding. [50, 100, 150]
9. Cannot assign to "finalPrice" because it is a constant. It causes an error since finalPrice is const and its the first const we try to reassign (can't do that).
10. Cannot assign to "finalPrice" because it is a constant. It causes an error since finalPrice is const and its the first const we try to reassign (can't do that). (won't reach)
11. Cannot assign to "finalPrice" because it is a constant. It causes an error since finalPrice is const and its the first const we try to reassign (can't do that). (won't reach here)
12. - A. student.name
    - B. student['Grad Year']
    - C. student.greeting()
    - D. student['Favorite Teacher'].name
    - E. student.courseLoad[0]
13. - A. '32' -> because the 2 gets converted to a string and added to '3' on arithmetic since we can do arithmetic on strings
    - B. 1 -> in this case the '3' gets converted to a number and the result is 1
    - C. 3 -> It gets converted to numbers where null becomes 0 resulting in just 3
    - D. '3null' -> It gets converted to strings so null becomes 'null' and it adds it to '3'
    - E. 4 -> true becomes 1 so 1 + 3 is 4
    - F. 0 -> in this case they both are converted to numbers and become 0
    - G. '3undefined' -> again, they get converted to strings
    - F. NaN -> We can't really do comparisons or stuff to undefined so it just becomes NaN as it becomes converted to it (to a number)
14. - A. true -> In this case the '2' becomes converted to a number resulting in true
    - B. false -> since both are string it compares letter by letter and '2' is not less than '1'
    - C. true -> '2' gets converted to a number
    - D. false -> because it is not strictly equal to each other, one is a string and the other is a number
    - E. true -> This is true because the 2 is a truthy value so true = true
    - F. true -> The 2 gets converted to a boolean and becomes true by the time they compare, so true === true
15. The difference between == and === is that the === needs to be stricly equal such as 2 and 2. But Lets say we have the number 2 and string '2', if we use == then we will get true since they get converted to match types etc. But '2' === 2 will be false since one is a number and the other is a string. 

<br>

17.. - We call the modifyArray with an array and a function, where we use the function (doSomething) to modify the contents of the array.
    - Then we declare a const newArr = [], this just means it will always point to an array but we can still modify the contents of it. 
    - Inside the loop we add to the inner contents of newArr the modified array[i] element (after passing it to the callback which is the doSomething function).
    - This way the inner contents of newArr will be the modified array.
    - Lastly we return the newArr

<b>
18.. - 1
    - 4
    - 3 
    - 2
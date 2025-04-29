1. values added: 20
2. final result: 20
3. The var is either function scoped or global scoped. So even though the var result was declared inside the if statement it 
was still accessable outside it. This is because the var was hoisted to the very top and declared there. It generally will be that way. This might be bad because you it becomes tricky to manage it and is generally better practice to use let/const instead because they are block scoped.
4. values added: 20
5. ReferenceError: result is not defined
    at sumValues (<anonymous>:16:33)
    at <anonymous>:19:1
    at mn (<anonymous>:16:5455)
    This is because we use let and it is block scoped inside the if statement and can only be accessed there. The console.log is outside of it and can't access it.
6. Cannot assign to "result" because it is a constant. We can't reassign a constant.
7. Cannot assign to "result" because it is a constant. We can't reassign a constant. (This line doesn't get reached because of the reassignment of a const)
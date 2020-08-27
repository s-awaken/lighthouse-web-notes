# Week_2 Day_4 Notes


*  callaback review
    *  callback hell
*  Intro to promises
*  error handling with promises (vs callbacks)
* creating promises

=== 

### 0. Review on Callbacks 

 - function that is passed as a parameter
 - helper function that you wait to use
 - can return a value but don't typically (especially when used asynchronously)
 - Async:
   - happens simultaeously (JS does one thing at a time)
   - executes after code has run
   - non blocking
   - runs code that we can complete
  
- Advantages of callbacks
  - code is modular
  - only way (currently) to handle async code
- Disadvantages
  - confusing to write
  - susceptable to callback hell

===

### 1. Promises


- something that is intended to get done
- can fulfill or break a promise
- commitment
- based on trust
- time element involved (do something in the future)
- agreement between one or more parties
-- all of these are applied to JS

=== JS Promise

three states: pending --> fulfilled or rejected

three values: undefined --> result: value or result: error


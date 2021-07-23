# JavaScript Call Stack and Error Messages

What is a ‘call’?
- Function invocation
How many ‘calls’ can happen at once?
- One
What does LIFO mean?
- Last in, First Out
Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```VM177:2 Uncaught Error: Stack Trace Error
    at firstFunction (<anonymous>:2:9)
    at secondFunction (<anonymous>:6:3)
    at thirdFunction (<anonymous>:10:3)
    at <anonymous>:13:1
```

What causes a Stack Overflow?
- A function that calls without exit point

What is a ‘refrence error’?
- variable not yet declared

What is a ‘syntax error’?
- data cannot by parsed with current syntax

What is a ‘range error’?
- error in length or data outside given range

What is a ‘tyep error’?
- data you are trying to access or use is incompatible by property/method

What is a breakpoint?
- The line in which the code can not longer execute

What does the word ‘debugger’ do in your code?
- causes a breakpoint
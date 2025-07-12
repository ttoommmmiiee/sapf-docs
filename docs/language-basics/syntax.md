---
sidebar_position: 2
---

# Syntax

Expressions are sequences of words (or other syntactic elements) written in postfix 
form. All words are are executed in left to right order as they are encountered. 
When a word is executed it looks up the value bound to that word. If the value is a 
function, then the function is applied and any arguments of the function are taken 
from the stack. If the value is not a function then the value itself is pushed onto 
the stack. 

```sapf
2 3 *           ; --> 6
4 1 0.4 +       ; --> 4 1.4
4 1 0.4 + +     ; --> 5.4
```


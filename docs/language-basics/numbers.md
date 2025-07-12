---
sidebar_position: 4
---

# Numbers

Numbers are written in the usual ways.
```sapf
1  2.3 .5 7.
```
    
Scientific notation
```sapf
3.4e-3  ; --> 0.0034
1.7e4   ; --> 17000
```

## Suffixes 
There are several suffixes that scale the value.

pi - scales the number by 3.141592653589793238...

pi can stand alone as well as being a suffix.
```sapf
pi      ; --> 3.14159
2pi     ; --> 6.28319 
.5pi    ; --> 1.5708 
.25pi   ; --> 0.785398
```     

M - mega. scales the number by one million 1000000.
```sapf
1M .5M ; --> 1000000 500000
```

k - kilo. scales the number by 1000.
```sapf
4k 1.5k ; --> 4000 1500
```

h - hecto. scales the number by 100.
```sapf
8h ; --> 800
```

c - centi. scales the number by .01
```sapf
386c 702c ; --> 3.86 7.02
```

m - milli. scales the number by .001
```sapf
53m 125m ; --> 0.053 0.125
```

u - micro. scales the number by .000001
```sapf
20u ; --> 0.00002
```

Infix fractions with no intervening spaces are interpreted as literal real 
numbers. Both the numerator and denominator can be floating point as 
described above.

```sapf
5/4     ; --> 1.25
9/7     ; --> 1.28571
15/11   ; --> 1.36364
pi/4    ; --> 0.785398
7.5/4   ; --> 1.875
1k/3    ; --> 1k/3
```
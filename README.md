# rpn
A console-based RPN calculator, inspired by the HP48 and HP42s.

# Commands (Operators)

```
     Symbol       # Args    Description
       +            2       add (x+y)
       -            2       subtract (x-y)
      * x           2       multiply (x*y)
       ^            2       power (x^y)
       /            2       divide (x/y)
    = == eq         2       equality (1 if x=y else 0)
   != !== ne        2       non-equality (0 if x=y else 1)
      not           1       0 if x != 0 else 1
      < lt          2       less than (1 if x<y else 0)
      > gt          2       greater than (1 if x>y else 0)
   <= le lte        2       less than or equal (1 if x<=y else 0)
   >= ge gte        2       greater than or equal (1 if x>=y else 0)
       <<           2       left shift (x<<y)
       >>           2       right shift (x>>y)
     mod %          2       modulus (x % y)
      abs           1       absolute value (|x|)
      sqrt          1       square root (sqrt(x))
      sum          all      sum of entire stack (x+y+z+w+...)
  product prod     all      product of entire stack (x+y+z+w+...)
     drop d        all      discard top item of stack
      swap          2       swap x and y on the stack
      dupe          1       make a copy of top item of stack
     _text          0       push 'text' onto stack
```

# Examples

```
   # rpn 1 2 +
   3.0000

   # rpn 1 2 3 4 5 sum
   15.0000

   # rpn 3 4 5 d +
   7.0000

   # rpn 2 sqrt
   1.4142

   # rpn 2 sqrt 2 '^'
   2.0000

   # rpn 1 2 '<'  (note: escape needed when using a shell)
   1.0000  # true

   # rpn 1 16 '<<'
   65536.0000

   # rpn 1 2 3
   1.0000
   2.0000
   3.0000
```

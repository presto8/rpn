# rpn
A console-based RPN calculator

# Commands (Operators)

```
Operator    Arguments    Description
   +            2        Add (x+y)
   -            2        Subtract (x-y)
   x *          2        Multiply (x*y)
   /            2        Divide (x/y)
   ^            2        Power (x^y)
   <<           2        Left shift (x << y)
   >>           2        Right shift (x >> y)
   <            2        Less than (1 if x < y else 0)
   >            2        Greater than (1 if x > y else 0)
   mod          2        Modulus (x % y)
   abs          1        Absolute value (|x|)
   sqrt         1        Square root (sqrt(x))
   sum        Stack      Sum of entire stack (x + y + z + w + ...)
   d            1        Drop 1 item from stack
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

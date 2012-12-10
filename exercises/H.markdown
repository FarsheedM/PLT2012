Programming Languages and Types

Exercise session H on 10.12.2012

Hand in

- anytime
- as a single Scala, Markdown or PDF file to pllecture@informatik, or
- in paper form during lectures or exercise sessions.

Solution will be posted before 17.12.12, 1400 hrs.

The tutor shall give feedback to each submission, without giving
points. Homework does not count toward course requirement. Do them for
your own benefit.

While everyone should write their own solution, it is recommended to
work face-to-face in small groups.


I. Monadic laws
===============

To qualify as a monad, one needs more than a type constructor and a
bind/return implementation of the correct type. In addition, monads
must respect the following three algebraic laws:

1. `(bind (return x) f)  == (f x)`
2. `(bind m return) == m`
3. `(bind (bind m f) g) == (bind m (lambda (x) (bind (f x) g)))`

Solve the following tasks.

a. Rephrase the laws in terms of do-notation.

b. Prove that the identity monad, the Maybe monad, and the Reader
   monad satisfy these laws.

c. Why do you think should monads obey these laws?


# Quadratic Equations Solver
This is module to solve quadratic eauation

# Usage Example
You should use python3.5
```
    [user@server]$ python3.5

    >>> from quadratic_equation import get_roots
    >>> print(get_roots(1,2,-1))
    (-2.414213562373095, 0.41421356237309515)

```
# Pre Commit Hook Usage
This hook is made to check validity of quadratic_equation code. It runs tests.py before commit to git and if tests fails commit won't proceed.

```
[user@server 14_pre_commit_hook]$ git commit -m "initial commit"
(-4.0, 1.0)
.E..
======================================================================
ERROR: test_returns_none_for_complex_solution (tests.QuadraticEquationTestCase)
----------------------------------------------------------------------
Traceback (most recent call last):
  File "/home/belov/devman/14_pre_commit_hook/tests.py", line 22, in test_returns_none_for_complex_solution
    root1, root2 = get_roots(1, 2, 3)
  File "/home/belov/devman/14_pre_commit_hook/quadratic_equation.py", line 6, in get_roots
    root1 = (-b - sqrt(discriminant)) / (2 * a)
ValueError: math domain error

----------------------------------------------------------------------
Ran 4 tests in 0.000s

FAILED (errors=1)

```


# Project Goals

The code is written for educational purposes. Training course for web-developers - [DEVMAN.org](https://devman.org)

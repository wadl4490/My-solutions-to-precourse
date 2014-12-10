## Python practice

We'll be getting more comfortable with Python built-in functions and data structures.

The course will heavily use Python for most of its analyses/projects.  It is not
necessary to be an expert in Python coming into the course (that is what we will
teach you!) but it is helpful to be familiar with it's syntax.

Not everyone knows Python (or what parts to focus on it in the classroom).  We
have provided resources here to get any student familiar with another
programming language up to speed with Python quickly (both in terms of syntax
and style). 

## Installing

We use the [Anaconda](https://store.continuum.io/cshop/anaconda/) Python 2.7
(not Python 3) distribution and use [conda](http://www.continuum.io/blog/conda)
to install any additional packages. You should install Anaconda now.

### Resources

If you still feel new to python, you might benefit from looking at one of these resources:
* [Dive Into Python](http://www.diveintopython.net/)
* [Learn Python the Hard Way](http://learnpythonthehardway.org/)

Please read through these [notes](python.md) which go over some more advanced python topics.

Python also has great documentation.

The [Python tutorial](https://docs.python.org/2/tutorial/) and
[Python library](https://docs.python.org/2/library/) are great resources if
you need to look up how something is done in Python.
    
## Assignment

#### 1. Practice with built-ins

Fill in the functions in `problems.py`.

These are all one-liners that use a bunch of handy built-in functions.

#### 2. Generating text

Fill in the functions `word_counts`, `associated_words` and `make_random_story`
in words.py. These will give you practice with reading files, strings and dictionaries.

Take a look at the [Collections module](https://docs.python.org/2/library/collections.html).
You may be able to use `DefaultDict` and `Counter` to simplify your code.

#### 3. Extra fun with Python

FizzBuzz is infamous for being a simple programming problem that [a lot of software
engineers struggle with](http://blog.codinghorror.com/why-cant-programmers-program/).

* Implement the function `fizzbuzz` in fizzbuzz.py. Don't worry, this is not the main point of this question.

* Modify the function definition so that the following calls all work. You should have 3 and 5 be the default parameters.
([documentation](https://docs.python.org/2/tutorial/controlflow.html#default-argument-values))

        fizzbuzz(15)                  # "FizzBuzz"
        fizzbuzz(15, fizz=4)          # "Buzz"
        fizzbuzz(15, buzz=4)          # "Fizz"
        fizzbuzz(15, fizz=6, buzz=7)  # ""

    Now in the main block you should be able to remove the 2nd and 3rd parameters.

* Look at how the main function uses `sys.argv`. You can run your program with this
command in the command line:

        python fizzbuzz.py 20

    Modify `words.py` so that you can run your program like this:

        python words.py alice.txt 200

    You'll have to import the `sys` module and use `sys.argv` ([documentation](https://docs.python.org/2/library/sys.html))

#### 5. Pandas

Resources:

* [10 Minutes to Pandas](http://pandas.pydata.org/pandas-docs/stable/10min.html)
* [Pandas top 10](http://manishamde.github.io/blog/2013/03/07/pandas-and-python-top-10/)

Pandas can be a very frustrating and mysterious library, it will be essential to get familiar with its quirks early on.

1. Complete the [pandas workshop](http://nbviewer.ipython.org/github/jvns/talks/blob/master/pydatanyc2013/PyData%20NYC%202013%20tutorial.ipynb) ([video](https://vimeo.com/79835526))


## What you should know

### Python

* Basic data structures and associated methods
  * int, float
  * string
  * list
  * dict
  * set
  * range
* Control structures
  * if, elif, else
  * while
  * for
  * break, continue, pass
* Enumerations
  * for loops
  * list comprehensions
  * enumerate
  * zip
* Functions
  * Declaration
  * Calling
  * Keyword arguments
* Object orientation
  * Classes
  * Methods
  * Properties (instance variables)
  * self
* Modules
  * import
  * aliasing (`import pandas as pd`)
  * global import (`from pandas import *`)
* IO
  * Read a file
  * Write to a file

Test yourself with these questions:

1. What's the difference between a list and a generator? And the advantages of either?
2. What is the advantage of storing a word list in a set rather than a list?

### NumPy

The NumPy workhorse is the `array` which is a high-performance matrix.

Think in matrices and matrix manipulation. Anything that can be vectorized
should be vectorized.

* Create: ones, zeros, eye, empty, random.random, random.randn
* size, shape, ndim
* min, max, mean, var
* Matrix multiplication
* Indexing, slicing, boolean indexing
* Broadcasting
* `np.linalg`: inv, det, solve, eig

### Pandas

* Series
* DataFrame
* Indexing, slicing, boolean indexing
* Broadcasting

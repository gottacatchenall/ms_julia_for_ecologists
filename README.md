
# Outline

- Why should ecologists learn julia?
    - Well, there are the criteria that are directly measureble that make it
      better than R/Python:
        - fast
        - native support on GPUs
    - But there are also criteria that are more subjective, and that take
      experience and practice using the language to appreciate
        - clever use of dispatch patterns 
        - use of one-lienrs
        - using parameterized types well
    - You will learn how to be a better programmer in _any_ language, because
      smart use of julia requires understanding some fundemantal concepts in
      programming that are 'hidden' from users in R/python
    - The biggest reason _not_ to use julia is that the ecology/evolution
      package ecosystem in R is larger, and the ML ecosystem in python is more popular. However:
        - you can call _any_ R/python function/library using RCall/PyCall in julia
        - More packages isn't necessarily better when they don't work together

---

# Abstract



---

# Introduction


In order to measure, understand, and mitigate the consequences of anthropogenic
change on ecosystems the serives they provide, ecologists need a set of
computational tools [@Urban2022CodLif]. These tools must be performant, but
crucially modular and interfaceable [@McIntire2022PerRei].

Constraints on have led to the so-called "two-language problem" in computational
science, where it is easier for a researcher to developer a prototype of a
model/simulation in a high-level language, like Python or R, and later have to
port the model to a lower-level compiled language because the performance of
these compiled languages (e.g. C++/Fortran) is orders of magnitude faster than
high level interpreted languages.



In fact, many of the most popular tools in higher-level languages are actually
thin wrappers around a compiled (often C++) base (e.g. tidyverse, keras, numpy,
TensorFlow, scikit-learn, pandas, etc.).

However, the skills required to use or debug---let alone write---scientific
software in these lower level langauges is not often taught. 

We propose that that Julia has certain properties absent in other popular
languages for scientific computing that make it particularly suited for the
development of a cohesive, modular, and extendible set of tools ideal for the
development of a platform for ecological analysis [@].




# The nature of computation in Julia

## Types

Why is this useful for ecologists? Often times in ecology, the same information
is represented in different formats. 
Two packages in R might not agree on what the "correct" format to represent
information is. 

**Concept fig here**



At the core of the Julia language is its _type system_. Type systems can often
be alienating to those who learned programming in so-called _dynamically_ typed
languages (like R, python, and JavaScript). In dynamically-typed languages,  `x=
5`, and `x = "hello world"` and the language won't care that you changed the
type of information that was stored in `x` from a number to a string.
Practically, this form of dynamic-typing was adopted because it is far more
convenient to write code like that above than defining variables with explicit
types, e.g. how you would in C: `char c = "a";` and `int x = 5;`. 


Julia doesn't require explicit type declarations, meaning `x = 5` is perfectly
valid code, but internallyJulia is doing the bookkeeping of what type of
information is stored in `x`, from an `Int64` to a `String` in the above
example.


Using explicit types is central to Julia's speed, but also enables much of its
most unique and user-friendly functionality, primarily the use of a
_multiple-dispatch_ system. 

## Dispatch

_Dispatch_ refers to the way a computer program decides what function to call. 

In many staticly-typed languages, you are allow to use the same function name
more than once. 


## Memory
4. Understand memory allocation 
5. Use broadcasting
6. Learn to debug and benchmark softare

# Doing computational science in `Julia`

## Managing Data

DataFrames.jl and DFMeta. 

## Doing statistics and machine learning

7. Learn about the statistics ecosystem: StatsBase, Statistics, GLM, MLJ, Flux,
   Turing 

## Doing simulation


8. Learn about the simulation libraries (DiffEq, DynamicGrids)
9. Learn how various statistics/simulation libraries work togethe

# Discussion 

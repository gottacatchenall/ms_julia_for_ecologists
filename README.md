
## Outline



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

10 rules to use julia effectively (highly tenative)

1. Use concrete types
2. Use abstract types
3. Learn about dispatch
4. Understand memory allocation 
5. Use broadcasting
6. Learn to debug and benchmark softare
7. Learn about the statistics ecosystem: StatsBase, Statistics, GLM, MLJ, Flux,
   Turing 
8. Learn about the simulation libraries (DiffEq, DynamicGrids)
9. Learn how various statistics/simulation libraries work together
10. Contribute to open-source community 
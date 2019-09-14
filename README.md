# Quadratic-Sieve
An implementation of the quadratic sieve algorithm for integer factorization. Can factorize 60 digit semiprimes in about 1 minute.

Usage:  

To use a single process for factorizing n:  

` pypy mpqs n `  

To use p processes:  

` pypy mpqs n p `  

To print progress of each process and keep printing estimated time remaining:  

` pypy mpqs n p 1 `  

Example: 

``` 
$ time pypy mpqs.py 1000000000100000000000000000074000000005700000000000000000969 4
Factorizing  61 digit number
Size of factor base ->  5459
Collecting data in parallel using 4 processes
Time taken to gather data ->  47.0951719284 seconds
Solving equations ...
Time taken to solve equations ->  17.254873991 seconds
1000000000100000000000000000074000000005700000000000000000969 = 1000000000000000000000000000057^1 * 1000000000100000000000000000017^1

real	1m4.559s
user	3m16.606s
sys	0m0.365s
```

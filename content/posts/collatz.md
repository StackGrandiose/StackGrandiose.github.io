---
title: Collatz Sequence 
date: 2024-01-11
tags: ['coding']
---

**[<-- Back]({{< ref "_index.md" >}})**

The website [ProjectEuler.net](https://projecteuler.net/) has many different math and logic based programming problems that
can be solved. In my attempt to deepen my understanding about coding and learn C, I decided to solve the problem relating to finding the
longest [Collatz Sequence](https://projecteuler.net/problem=14). The following program was compiled using gcc.

```

#include <stdio.h>

long evenOperation (long n) {
    n = n / 2;
    return(n);
}

long oddOperation (long n) {
    n = (3*n) + 1;
    return(n);
}

int main (int argc, char **argv) {
    long number = 0;
    long maxPathLength = 0;
    long maxLengthInt = 0;
    long numOfTerms = 100;

    for (int i = 0; i < numOfTerms; i++) {
        long currentLength = 1;
        while (number > 1) {
            if ((number % 2) == 0) {
                number = evenOperation(number);
                currentLength++;
            }
            else {
                number = oddOperation(number);
                currentLength++;
            }
        }
        if (currentLength > maxPathLength) {
            maxPathLength = currentLength;
            maxLengthInt = i-1;
        }
        number = i;
    }
    printf("TERM: '%li' WITH A SEQUENCE LENGTH OF '%li'\n", maxLengthInt, maxPathLength);
    return(0);
}

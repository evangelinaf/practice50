# Encryption

## Prerequisites
None

## Problem
An encryption application requires you to first input two integers that are larger than 100, one of which is a multiple of 7 and one of which is a multiple of 19. Add two functions to the code below which verify that the input meets the required criteria, and return true/false.  

## Distribution Code
```c
#include <cs50.h>
#include <stdio.h>

// TODO: Write function prototypes


int main(void)
{
    // query user for input
    printf("enter the first encryption factor: ");
    int fac_1 = get_int();
    printf("enter the second encryption factor: ");
    int fac_2 = get_int();
    // print result
    if (test_7(fac_1) && test_19(fac_2))
        printf("Success! Message was encrypted\n");
    else
        printf("Factors failed. Please try again later\n");
}

// TODO: Write function definitions

```
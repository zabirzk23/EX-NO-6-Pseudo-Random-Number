# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: \n");
    scanf("%d", &count);
    printf("Enter the minimum value:\n");
    scanf("%d", &min);
    printf("Enter the maximum value:\n");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d ", random_number);
    }
    return 0;
}

```
# OUTPUT:

<img width="557" height="315" alt="Screenshot 2025-09-17 094831" src="https://github.com/user-attachments/assets/6577f081-5397-4fa3-939a-670428f78afe" />

# RESULT:

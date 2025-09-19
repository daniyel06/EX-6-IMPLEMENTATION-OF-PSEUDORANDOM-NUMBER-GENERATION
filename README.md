## EX: 6 IMPLEMENTATION OF PSEUDORANDOM NUMBER GENERATION 
## NAME: DANIYEL ANTONY RAJ SD
## REGISTER NO: 212224220018

## AIM:
To Implement Pseudorandom Number Generation Using Standard library.


## ALGORITHM:

1.	Start the program and import the required libraries.
2.	Seed the random number generator using the current time (i.e) rand(time(0));
3.	Get the number of random numbers to generate.
4.	Pass the value for number of iterations and print the numbers.
5.	End the program.


## PROGRAM:
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    int count, min, max;

    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);

    printf("Enter the minimum value: ");
    scanf("%d", &min);

    printf("Enter the maximum value: ");
    scanf("%d", &max);

    srand(time(NULL));

    printf("Pseudorandom numbers:\n");
    for (int i = 0; i < count; i++) {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }

    return 0;
}

```

## OUTPUT:
<img width="810" height="600" alt="image" src="https://github.com/user-attachments/assets/5f72e414-0fd5-4332-914e-0f558d7c6561" />


## RESULT:
The Implementation of Pseudorandom Number Generation Using Standard library is successful.

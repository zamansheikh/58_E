### Answer No: 2

There are several types of control flow structures available:

1. **Sequential Control:** Statements in C are executed in sequence, one after another, by default. This is the default control flow where each statement is executed in the order they appear.

    ```c
    int a = 5;
    float b = 3.14;
    printf("Value of a: %d\n", a);
    printf("Value of b: %f\n", b);
    ```

2. **Selection Control (Conditional Statements):** These control structures allow the program to make decisions based on conditions. The commonly used conditional statements in C are:
   
    a. **if Statement:**
    
    ```c
    int num = 10;
    if (num > 0) {
        printf("Number is positive.\n");
    } else {
        printf("Number is non-positive.\n");
    }
    ```

    b. **if-else if-else ladder:**
    
    ```c
    int num = 10;
    if (num > 0) {
        printf("Number is positive.\n");
    } else if (num < 0) {
        printf("Number is negative.\n");
    } else {
        printf("Number is zero.\n");
    }
    ```

    c. **switch Statement:**

    ```c
    int choice = 2;
    switch (choice) {
        case 1:
            printf("Choice is 1.\n");
            break;
        case 2:
            printf("Choice is 2.\n");
            break;
        default:
            printf("Invalid choice.\n");
    }
    ```

3. **Repetition Control (Loops):** These control structures allow executing a block of code repeatedly based on certain conditions.
   
    a. **for Loop:**

    ```c
    for (int i = 0; i < 5; i++) {
        printf("Value of i: %d\n", i);
    }
    ```

    b. **while Loop:**

    ```c
    int count = 0;
    while (count < 5) {
        printf("Count: %d\n", count);
        count++;
    }
    ```

    c. **do-while Loop:**

    ```c
    int x = 0;
    do {
        printf("Value of x: %d\n", x);
        x++;
    } while (x < 5);
    ```

4. **Jump Statements:** These allow altering the normal flow of a program by transferring control to another part of the code.
   
    a. **break Statement:** Used to exit a loop or switch statement.
    ```c
   #include <stdio.h>

    int main() {
        int i;
        for (i = 1; i <= 10; i++) {
            if (i == 5) {
                break; // Exit the loop when i equals 5
            }
            printf("%d\n", i);
        }
        return 0;
    }
    ```
   
    b. **continue Statement:** Skips the current iteration of a loop.
    ```c
    #include <stdio.h>
    
    int main() {
        int i;
        for (i = 1; i <= 5; i++) {
            if (i == 3) {
                continue; // Skip printing when i equals 3
            }
            printf("%d\n", i);
        }
        return 0;
    }
    ```
   
    c. **goto Statement:** Transfers control to a labeled statement in the program.
    ```c
   #include <stdio.h>
   int main() {
      int i = 0;
      
      loop:
      i++;
      if (i <= 5) {
          printf("%d\n", i);
          goto loop; // Jump to the 'loop' label
      }
      return 0;
    }
    ```

Control flow structures in C provide the ability to create dynamic and flexible programs by controlling the execution sequence based on conditions and loops.

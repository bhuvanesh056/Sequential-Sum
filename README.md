# Sequential-Sum
## AIM:
To write an Assembly Language Program (ALP) in 8051 to calculate the sum of 5 numbers stored sequentially in memory and store the result in another memory location.

## APPARATUS REQUIRED:
1.Keil µVision Software / 8051 Simulator

2.Personal Computer

## ALGORITHM:
1.Initialize the data pointer to the starting address where the numbers are stored.

2.Initialize a register or accumulator to 00H to store the sum.

3.Load each number sequentially from memory and add it to the accumulator.

4.Repeat this process for all 5 numbers.

5.Store the final result in another memory location.

6.Stop the program execution.

## PROGRAM:
```
ORG 0000H
MOV R0, #30H
MOV R2, #05H
CLR A

BACK: ADD A, @R0
INC R0
DJNZ R2, BACK

MOV 35H, A
END
```

## OUTPUT:

![WhatsApp Image 2025-10-25 at 09 50 38_b679d106](https://github.com/user-attachments/assets/f8cfeefb-f630-43ef-9b0b-2eeda35d8081)

## RESULT:
The program has been successfully executed.

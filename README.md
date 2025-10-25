# Sequential-Sum
## AIM:
To write an Assembly Language Program (ALP) in 8051 to calculate the sum of 5 numbers stored sequentially in memory and store the result in another memory location.

## APPARATUS REQUIRED:
1.Keil µVision Software / 8051 Simulator

2.Personal Computer

## ALGORITHM:
1.Start the program.

2.Initialize R0 with the starting address (30H) where numbers are stored.

3.Load R2 with count value 05H (since there are 5 numbers).

4.Clear the accumulator (A) to start summation from zero.

5.Fetch the number from memory pointed by R0.

6.Add the fetched number to the accumulator.

7.Increment R0 to point to the next memory location.

8.Decrement R2 and repeat steps 5–7 until R2 = 0.

9.After the loop ends, store the final sum in memory location 35H.

10.End the program.

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

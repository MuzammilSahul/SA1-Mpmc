# SA1-Mpmc(21224060162)

## AIM:

   To Write an assembly language program in 8051 to exchange the contents of two memory blocks of equal length.
---
## APPARATUS REQUIRED:

   - PERSONAL COMPUTER
    
   - Keil Vision
---
## ALGORITHM
1. Source and estination location addresses are loaded to register R0 and R1 respectively.
2. Number of bytes to be transferred is loaded into register R2.
3. Copy the data from source location to register B.
4. Load the data from destination location to source location.
5. Now transfer content of register B to destination location.
6. Repeat the process until all the bytes are exchanged between the source and destination location.
---
  ## PROGRAM:

  ASSEMBLY LANGUAGE PROGRAM IN 8051 TO EXCHANGE CONTENTS OF TWO MEMORY BLOCKS IN EQUAL LENGTH

```asm

ORG 00H
SJMP 30H
ORG 30H
MOV R0,#30H
MOV R1,#40H
MOV R2,#05H
LOOP:MOV A,@R0
MOV B,A
MOV A,@R1
MOV @R0,A
MOV A,B
MOV @R1,A
INC R0
INC R1
DJNZ R2,LOOP
HERE:SJMP HERE
END

```
---
## OUTPUT:

## 1.BEFORE MEMORY EXCHANGE:
<img width="663" height="877" alt="Screenshot 2025-10-24 210859" src="https://github.com/user-attachments/assets/54739760-543b-4943-be2d-c65daaa4aed1" />
<img width="536" height="866" alt="Screenshot 2025-10-24 210951" src="https://github.com/user-attachments/assets/42f36f0a-a297-4314-a5c1-8493d143ea73" />


## 2.AFTER MEMORY EXCHANGE(RUNNING THE PROGRAM):
<img width="610" height="867" alt="Screenshot 2025-10-24 211032" src="https://github.com/user-attachments/assets/597e1cf3-8f06-43c0-b380-7bb34bb087bd" />

<img width="506" height="860" alt="Screenshot 2025-10-24 211004" src="https://github.com/user-attachments/assets/7029f348-f621-45b3-b981-0fa2e3e3543f" />
---

## RESULT:

Thus the program  to exchange thecontents of two memory blocks of equal length is done and output is displayed.

---
  
  

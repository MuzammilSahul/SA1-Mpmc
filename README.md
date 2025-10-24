# SA1-Mpmc

## AIM:

   To Write an assembly language program in 8051 to exchange the contents of two memory blocks of equal length.
---
##APPARATUS REQUIRED:

   - PERSONAL COMPUTER
    
   - Keil Vision
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
  
  

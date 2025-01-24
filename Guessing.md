# Guessing Game
 In this game, the computer will randomly select a number from one to five.
 The person will try to guess the number the computer randomly selected.
## ONLY numbers between one and five will be accepted.
 If the user enters anything outside of the numbers one through five, they will be prompted:
## NUMBERS 1-5 ONLY
 Then the user will be redirected back to try to guess the number.
 If the user gets the number wrong, they will be prompted:
## WRONG, TRY AGAIN!
 The process will continue until the computer guesses the number correct three times in a row.
 Once the copmuter successfully guesses the numer three times in a row, a message pops up saying
## !!CONGRATULATIONS!!

```mermaid
flowchart TD
A ~~~ B
A[COMPUTER selectes random number 1-5] -->C{MATCH 1}
B[USER 1st attempt at selecting number 1-5] ==>|Correct Guess|C
B .->|anything outside 1-5|D(**NUMBERS 1-5 ONLY**)
D -->B
C ==>E[USER 2nd attempt at selecting number 1-5]
E ==>|Correct Guess|F{MATCH 2}
A -->F
B .->|Inorrect Guess|H{**WRONG, TRY AGAIN!**}
F ==>G[USER 3nd attempt at selecting number 1-5]
H -->B
E .->|Inorrect Guess|H
G ==>|Correct Guess|I{**!!CONGRATULATIONS!!**}
A -->I
G .->|Incorrect Guess|H
```

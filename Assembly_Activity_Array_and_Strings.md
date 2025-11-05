# Array and Strings

This activity will be done per the FINAL PROJECT groupings already assigned.

Design an Assembly program that allows the user to choose between handling numbers or words. The program must:

Accept either:

Five positive integers, OR

Five words (max 10 chars each)

Values must be stored in arrays.

For integers:

Store the five numbers in an array

Display both the sorted ascending and descending versions

For words:

Store the five words in an array of strings

Convert each word by replacing all vowels with numbers

(a→1, e→2, i→3, o→4, u→5, both uppercase and lowercase)

Sort the converted words in:

lexicographically ascending

lexicographically descending

String instructions constraint:

You must use at least one x86 string instruction (e.g. LODSB, STOSB, MOVSB, SCASB, or CMPSB).

Program structure and documentation:

Use proper .data, .bss, .text section labels

Include comments explaining each line of code

Use modular programming with procedures

Display an error message for invalid menu choices

Looping behavior:

After finishing each task, return to the main menu

The program exits only when the user selects 0



Documentation must include:

A complete sample run for:

Sorting numbers

Sorting and vowel-replacing words

Only one member submits the final documentation

Upload a YouTube video recording a sample run. Group members' faces must be visible.


## SAMPLE RUN:

```
MENU:

[1] Enter five numbers

[2] Enter five words

[0] Exit

Enter choice: 5

ERROR: Invalid menu choice. Please try again.



MENU:

[1] Enter five numbers

[2] Enter five words

[0] Exit

Enter choice: 1



Enter integer #1: abc

ERROR: Input is not a valid integer. Please re-enter.

Enter integer #1: -12

ERROR: Only positive integers are allowed. Please re-enter.

Enter integer #1: 25

Enter integer #2: 14

Enter integer #3: 9

Enter integer #4: x7

ERROR: Input is not a valid integer. Please re-enter.

Enter integer #4: 7

Enter integer #5: 30



Numbers entered: 25 14 9 7 30

Ascending : 7 9 14 25 30

Descending: 30 25 14 9 7



Returning to main menu...



MENU:

[1] Enter five numbers

[2] Enter five words

[0] Exit

Enter choice: 2



Enter word #1: app13

ERROR: Words may only contain letters. Please re-enter.

Enter word #1: apple

Enter word #2: orange

Enter word #3: ***

ERROR: Words may only contain letters. Please re-enter.

Enter word #3: table

Enter word #4: U N I T

ERROR: Words cannot contain spaces. Please re-enter.

Enter word #4: UNIT

Enter word #5: chalk



Converted words:

apple  → 1ppl2

orange → 4r1ng2

table  → t1bl2

UNIT   → 5n3t

chalk  → ch1lk



Sorted ascending:

1ppl2

4r1ng2

5n3t

ch1lk

t1bl2



Sorted descending:

t1bl2

ch1lk

5n3t

4r1ng2

1ppl2



Returning to main menu...



MENU:

[1] Enter five numbers

[2] Enter five words

[0] Exit

Enter choice: 0

Program terminated.
```

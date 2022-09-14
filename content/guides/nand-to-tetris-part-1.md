+++
title = "Build a Modern Computer from First Principles: From Nand to Tetris"
weight = 50
+++
---

## Getting started

Nand to Tetris is a course that has you build a simplified computer from basic electrical
components. The course is split into 2 parts: part 1 (this course) focuses
on the physical parts of the computer and part 2 is concerned with the software
implemented on top of the hardware. 

## Prerequisites

There aren't clearly defined prerequisites for this course, but you actually need to know a lot of little bits and pieces of things (that people struggled with).

First of all, you will be writing an assembler, which is a program that takes one language as input and produces code in another language as output. And you need to write this program in a third language (like Python or Java). So you need to already have very solid knowledge of one programming language, how to do file read/write and how to process strings in that language. You'll also need to know some data structures (like a dictionary in Python) because the assembler will need to look up some values in a symbol table.

Second, you need solid logic and Boolean algebra skills, and you need to know how to work with binary numbers and bits. Otherwise you'll have a lot of trouble translating the project instructions to chips, and the chips you implement will be extremely difficult to debug. I've seen this happen to a few people.

Third, you'll be using a hardware description language, which looks like a programming language but doesn't act like a programming language. So you'll need a different way of thinking there. I've seen many people make mistakes because they treat it like a programming language.

There are probably some other "hidden" prerequisites that might not be included above.

## Assignments

{{< tip >}}
Some of the assignments can be tedious to do manually so you could write small
scripts to help you like the one below.
{{< /tip >}}

```python
for i in range(0, 16):
    print(f"And(a=a[{i}], b=b[{i}], out=out[{i}]);")

# The preceding code outputs:

# And(a=a[0], b=b[0], out=out[0]);
# And(a=a[1], b=b[1], out=out[1]);
# And(a=a[2], b=b[2], out=out[2]);
# And(a=a[3], b=b[3], out=out[3]);
# And(a=a[4], b=b[4], out=out[4]);
# And(a=a[5], b=b[5], out=out[5]);
# And(a=a[6], b=b[6], out=out[6]);
# And(a=a[7], b=b[7], out=out[7]);
# And(a=a[8], b=b[8], out=out[8]);
# And(a=a[9], b=b[9], out=out[9]);
# And(a=a[10], b=b[10], out=out[10]);
# And(a=a[11], b=b[11], out=out[11]);
# And(a=a[12], b=b[12], out=out[12]);
# And(a=a[13], b=b[13], out=out[13]);
# And(a=a[14], b=b[14], out=out[14]);
# And(a=a[15], b=b[15], out=out[15]);
```
Week 06 of the course requires you to write an assembler for the Hack assembly.
These are the relations of the symbolic to binary representation of the Hack commands.

The destination field of the *C* instruction:
```json
{
"null": "000",
"M": "001",
"D": "010",
"MD": "011",
"A": "100",
"AM": "101",
"AD": "110"
}
```
The jump field of the *C* instruction:
```json
{
"null": "000",
"JGT": "001",
"JEQ": "010",
"JGE": "011",
"JLT": "100",
"JNE": "101",
"JLE": "110",
"JMP": "111",
}

```
The comp field of the *C* instruction:
```json
{
"0": "0101010",
"1": "0111111",
"-1": "0111010",
"D": "0001100",
"A": "0110000",
"!D": "0001101",
"!A": "0110001",
"-D": "0001111",
"-A": "0110011",
"D+1": "0011111",
"A+1": "0110111",
"D-1": "0001110",
"A-1": "0110010",
"D+A": "0000010",
"D-A": "0010011",
"A-D": "0000111",
"D&A": "0000000",
"D|A": "0010101",
"M": "1110000",
"!M": "1110001",
"-M": "1110011",
"M+1": "1110111",
"M-1": "1110010",
"D+M": "1000010",
"D-M": "1010011",
"M-D": "1000111",
"D&M": "1000000",
"D|M": "1010101",
}
```
The symbol table for the built in labels:
```json
{
"R0": 0,
"R1": 1,
"R2": 2,
"R3": 3,
"R4": 4,
"R5": 5,
"R6": 6,
"R7": 7,
"R8": 8,
"R9": 9,
"R10": 10,
"R11": 11,
"R12": 12,
"R13": 13,
"R14": 14,
"R15": 15,
"SP": 0,
"LCL": 1,
"ARG": 2,
"THIS": 3,
"THAT": 4,
"SCREEN": 16384,
"KBD": 24576,
}
```

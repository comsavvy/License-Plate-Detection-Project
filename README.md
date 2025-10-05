# African Institute for Mathematical Sciences (AIMS)

## Python Programming (PP) Project: Senegalese Vehicle License Plate Detector

### Objectives:

Write a program in pure Python (no external libraries) that detects the presence of Senegalese vehicle license plate numbers inside any text string. 

We consider the following formats (letters are A–Z; digits are 0–9):

XY-abcd-T or XY-abcd-ZT

where X, Y, Z, T are letters and a, b, c, d are digits.

### Requirements
1. The input is an arbitrary string; the output is a Boolean. If True, the program must also print all detected license plates.
2. Matching is case-insensitive; detected plates must be normalized to uppercase and printed in canonical hyphenated form XY-ABCD-T/XY-ABCD-ZT.
3. Allow either a hyphen or a single space as a separator (- or ). For example, XY 1234 T and xy-1234-zt must be recognized and normalized.
4. Do not match substrings embedded within longer alphanumeric tokens (e.g., do not match across letters/digits without a boundary).
5. If multiple plates appear, print them in the order they appear, without duplicates.
6. If no plate is found, print a clear message stating so.

### Additional Complexity
- Tolerate trailing punctuation around a plate (e.g., commas or periods).
- Count and display the total number of unique plates found at the end.
- Provide a minimal text menu to test multiple inputs until the user quits.
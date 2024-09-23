## Braille Translator
In this mini project I will create a terminal / command-line application that can translate Braille to English and vice versa. 

The string to translate will be passed into your application as an argument at runtime. Your application must be smart enough to determine if the string given to it is either Braille or English and automatically convert it to the appropriate opposite. 

For the purposes of this project Braille must be displayed as `O` and `.` where `O` represents a raised dot. I must include the entire English alphabet, the ability to `capitalize` letters, add `spaces`, and the numbers `0` through `9` as well. 

After conversion, output the translated string--and nothing else--to the terminal. 

## What is Braille?
Braille (*/breɪl/ **BRAYL***) is a tactile writing system used by people who are visually impaired. Braille characters are formed using a combination of six raised dots arranged in a 3 × 2 matrix, called the braille cell. The number and arrangement of these dots distinguishes one character from another. ([via Wikipedia](https://en.wikipedia.org/wiki/Braille))

<p align='center'>
  <img src='./braille.jpg' alt='Braille Alphabet' />
</p>
<p align='center'>
  <em style='font-size:xx-small;'>Black dots represent raised areas</em>
</p>

## Technical Requirements
- Translator
  - Given arguments passed into the program at runtime, determine if the given string should be translated to English or Braille.
  - For Braille, each character is stored as a series of `O` (the letter O) or `.` (a period).
  - Store Braille symbols as a 6 character string reading left to right, line by line, starting at the top left. See examples below.
  - When a Braille `capital follows` symbol is read, assume only the next symbol should be capitalized. 
  - When a Braille `number follows` symbol is read, assume all following symbols are numbers until the next `space` symbol.
- Braille Alphabet
  - Letters `a` through `z`
    - The ability to capitalize letters
  - Numbers `0` through `9`
  - The ability to include `spaces` ie: multiple words

## Examples
- Launching your application with English or Braille:
  - `ruby translator.rb Hello world`
  - `ruby translator.rb .....OO.OO..O..O..O.O.O.O.O.O.O..OO........OOO.OO..OO.O.OOO.O.O.O.OO.O..`
---
- Input: `Hello world`
- Output: `.....OO.OO..O..O..O.O.O.O.O.O.O..OO........OOO.OO..OO.O.OOO.O.O.O.OO.O..`
---
- Input: `42`
- Output: `.O.OOOOO.O..O.O...`
---
- Input: `.....OO.....O.O...OO...........O.OOOO.....O.O...OO....`
- Output: `Abc 123`

## Instructions
1. Fork this repo to your personal Github Account
1. Clone your forked repo to begin working on the challenge locally.
2. Try to run the command line: cd python | ./translator.py <Braile/English sentence>

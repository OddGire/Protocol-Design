# Protocol-Design
A design for a project for ICS2OI (Grade 10 Computer Science).
## Legend
- Side 1: The side that's communicating the data.
- Side 2: The side that's interpreting the data
## Setup
- Side 1 gets an orange flag, black flag, white flag and the 10x10 image.
- Side 2 gets a red and green flag as well as a 10x10 grid to fill in the pixels.
## Rules
Side 1 raises the orange flag to start. Side 1 then uses flags to say how many pixels in a row are filled or not filled. A chart with each colour and ther respective orders detrmine how many pixels in a row are of that colour like the following:
| Number of pixels in a row | Colour combination |
| ------------------------- | ------------------ |
| 1 | The colour (black or white) |
| 2 | Black, White |
| 3 | Black, Orange |
| 4 | White, Orange |
| 5 | White, Black |
| 6 | Orange, White |
| 7 | Orange, Black |
| 8 | Orange, Black, White |
| 9 | Black, Orange, White |
| 10 | Orange, White, Black |

If a pixel is repeated more than 10 times in a row, the combination "Black, White, Orange" will be used to show the repition of colours. A single orange flag is used to show the start of the flag raises, an error or the end of the flag raises.
Side 2 uses their red flag to indicate the side 1 to repeat their previous flag raise and a green flag to move on to their next flag.

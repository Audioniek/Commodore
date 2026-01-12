B-keyboard ROM images

The 40 column ROMs for the B-keyboard are direct descendants
of the Commodore original ROMs for the FAT40 (ROMs 901498-01
and 901499-01 respectively) with the following changes:

- The keyboard decoding table is the same as that for the 40 column
  9 inch CRT models with a B-keyboard;
- The key handling for shifted keys is the same as that for the 40 column
  9 inch CRT models wuth a B-keyboard;
- The CRT mode after power up is text.

The rest of the features have been retained unchanged; the key REPEAT will repeat
the key pressed simulatiously with it.

The bug in the processing of shifted keys with decimal mode set has not
been corrected on purpose, as all original Commodore ROMs feaure it. The
reason for this is to assure maximum compatibility with all other ROMs.



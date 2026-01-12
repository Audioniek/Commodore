N-keyboard ROM images

The 80 column ROMs for the N-keyboard are direct descendants
of the Commodore original ROMs for the 8032 (ROMs 901473-01
and 901474-01 respectively) with the following changes:

- The keyboard decoding table is the same as that for the 40 column
  FAT40;
- The key handling for shifted keys is the same as that for the 40 column
  FAT40;
- The CRT mode after power up is graphics.

The rest of the features have been retained unchanged, including
the support for a screen window.

The processing for the following features has been changed because
of the keyboard differences:
- Cancel quote mode: press unshifted RUN/STOP;
- Slow scroll: press space bar;
- Freeze scroll: press unshifted RVS (release freeze: press space bar);
- Repeating keys are controlled by the value of memory location $E4 (244):
  $40 (bit 6 on): no keys repeat;
  $0 (bit 6 off): all keys repeat;
  $80 (bit 7 on): only space, cursor left/right, cursor up/down and INS/DEL
  repeat (default after power on).


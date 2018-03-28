# Circuits

These were my solutions to an assignment on various circuits as part of a Computer Systems Architecture module at the University of Brighton.

All of these circuits can only handle 4 bit numbers, but could potentially be extended to any word size.

To test these circuits, they have to be run in Digital Works (https://www.mecanique.co.uk/shop/index.php?route=product/category&path=89), a relatively out-dated program that just about works.

## Divider problem

The only known problem with this circuit is within the divider; when -8 / -8 occurs, the output is -1, rather than 1. The cause of this is due to the circuit converting to twos complement before a negative division occurs: -8 (1000 in binary) cannot be converted to +8 using only 4 bit binary, so a carry occurs. The divider cannot currently handle this carry. I may, however, find a solution to this at a later date.

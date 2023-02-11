# How to Make Lego Dimensions NFC Tags

1) Read the blank tag.
2) Write down the first 6 characters from Addr. 00 (aka 0x00).
3) Write down the 8 characters from Addr. 01 (aka 0x01).
4) Combine the characters from steps 2 and 3 into one string in the order they
   were collected.
5) Open the following website: https://ldcharcrypto.ags131.com/
6) Input the string created from step 4 as the `UID` in the website opened from step 5.
7) Input the character/vehicle ID of the desired character/vehicle in the website from
   step 5.

   These IDs can be found in the `.csv` files in the same directory as this file.
8) Hit the `calculate` button on the website. Write down the results.
9) The two tag types (NFC213 and NFC215) this document is specifically written
   for differ in where the password value is to be saved.

   If the blank tag to be written to is a 213 NFC tag, edit the tag as the
   results say.

   If the blank tag to be written to is a 215 NFC tag, edit the (0x24) and
   (0x25) as the results say. For the (0x2B) address, instead edit the (0x85)
   address with that hex code.

## Example Calculation

Step 2) 04978F

Step 3) 22287380

Step 4) 04978F22287380

Step 7) ID 4

Step 8)

    35 (0x23) 00000000

    36 (0x24) 73492BB8

    37 (0x25) F35F482C

    38 (0x26) 00000000 (Token Type)

    43 (0x2B) 9B2571FE

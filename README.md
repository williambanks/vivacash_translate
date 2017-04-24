# cashola_translate

The idea behind Cashola is to make it possible to send money to anyone, anywhere in the world with little more than a "HELLO" in their local language.

Cashola's focus is on simplicity and ease of use.
In order for Cashola to support a new language it must have a string table for that language.

At the present time we only have English and are asking the community to help with translations by forking the project here on github and creating their own translation file.

In order to contribute, you just fork the project, create a new language file that matches the english one, change out the wording and submit a pull request.

The way we name files is "language.strings.json" with language being a reference to the 2 digit [ISO 639-1 code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the language.

Every word should be changed to match the local language.

They say brevity is the soul of wit, and brevity is extremely important when it comes to SMS.
The longest message we can possibly deliver is 130 bytes.
But if the language requires "non-ascii" characters, then the length of a line should not exceed 70 characters, because unicode characters consume 2 bytes each, plus there is some overheard in signaling the phone to switch to the correct characterset.

Variables are represented as $1, $2 and $3 etc.  You must account for variable names when considering your translation.
Phone numbers can consume up to 15 digits,and the longest currency name we support is "VIVA CROWNS" which is 11 characters.
Therefore if possible you should try to keep the descriptions in the help section of each file to no more than 70 characters regardless of if it's ascii or unicode.

This README file also doubles as a directory for Cashola
So please check this page for up to date number lists and if you'd like to see a country supported, please make sure we have a language file for that country and then open an issue requesting your country be added to the list of countries we support.

This project provides the language translations for Cashola SMS and bot menus

cashola.me is the easiest way to send or receive money worldwide.


| Country           | Number           | 
|-------------------|------------------|
| USA LIVE          | 14063156123      |  
| USA BETA          | 12016219467      |
| Germany BETA      | 4915735992274    |
| South Africa Beta | 2787240508610101 |

The difference between a live number and a beta number is that a beta number will not actually send funds.  They are otherwise identical and an account created and managed on a beta line, will become live automatically when the number is switched from beta to live.  We will try to give a couple of days warning in the issues section here when we do move a number from beta to live.

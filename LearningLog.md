# *My Learning Log*
I thought about logging everything I do and everything I learn + struggles and other things (we'll see).

I think doing this day by day is a good basis and probably fun to look back on too.

I'm also going to be writing the main thing I worked on that day and next to it a counter for how many days I've worked on that specific thing (e.g. `Python #1, Linux #5`)


***'xx:xx'*** refers to the time I began writing the log.

***'Things I learned'*** refers to a thing, or things, that I now know how to do (that I previously didn't). I feel like I'm gonna mess up the formatting as this continues, but so be it.

***'xh spent'*** refers to, well, the amount of hours I spent studying/learning/building/whatever-else-related that day.

## *31.10.2026*

***Python #1***

This is not my first day learning nor doing things, but this will be the starting point to my log.

***17:30***: I'm currently working on a password checker in Python. You give it an input (a password), and it's supposed to tell you what is missing and how strong it is. Currently I've finished the functions to check length, lowercasing and uppercasing. You can find it on my github page under the name `Python-Password-Checker` or just paste the link `https://github.com/NoamSilander/Python-Password-Checker`.

***18:08***: I finished creating the log base, I'm gonna continue writing the checker. 

***18:52*** I built the first complete version of the password checker and pushed it to GitHub.

***19:01*** Taking a break (maybe stopping for today)

***Things I learned:***
- `islower()`: checks if said character is lowercase (if yes, returns `True`)
- `isupper()`: checks if said character is uppercase (if yes, returns `True`)
- `isdigit()`: checks if said character is a digit (if yes, returns `True`)
- `isalnum()`: checks if said character is a digit or a letter (if yes, returns `True`)
- You can write conditional variables in Python `answer = 'yes' if correct else 'no'`
- You can print lists cleanly by using `.join()` (e.g. `print', '.join(list_name)`). The characters inside the quotes (`', '`) act as the glue between each item in the list. (What comes between each one)
- You can check if a list is empty by writing `if not list_name:`

***2h spent***

## 01.11.2026

***Python #2***

***17:37*** I began work on a password generator (since it fits yesterdays project of a password checker)

**19:34** I finished building the password generator and pushed it to GitHub under the name `Python-Password-Generator`. You can also paste the link `https://github.com/NoamSilander/Python-Password-Generator`. Taking a break.

***Things I learned:***
- `import random` is not good for real security and passwords, because it's randomness algorithm is predictable and seedable. For real password generation, use `import secrets` which gives 'truly' random numbers. You use it by writing `secrets.choice(your_string)` and it gives you one character from it at random.
- `import string` which is a module that has ready made strings (thus the name). `string.ascii_letters` gives `abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ`, `string.digits` gives `0123456789`, and `string.punctuation` gives `!"#$%&'()*+,-./:;<=>?@[\]^_'{|}~` (I had to replace ` with ' for it to properly format in Markdown.)

***2h spent***

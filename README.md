# *My Learning Log*
This is a README copy of the original log. (So it appears neatly in the repo.)

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

## 02.11.2026

***11:51*** I began studying `with` and the `open()` function to prepare for building a saving TO-DO list.

***12:45*** I finished getting familiar with `open()` and began working on the TO-DO list.

***14:38*** I got the TO-DO list about 70% done. College ended so I'm taking a break until I return home.

***Things I learned:***
- using `\n` after a string makes the next one start on a new line (e.g. print('first line\n second line'))
- `with open('file', 'mode', 'encoding') as variable:` is the structure. `with` also closes the file immediatly once the body ends.
- `open()` modes include `r` = **read the file**, `w` = **wipe the file and write**, `a` = **append (write to the end without wiping)**, `x` = **exclusive creation (Only allows if file doesn't exist. Raises `FileExistsError`)**

***3h spent***

## 03.11.2026

***Python #4***

***10:34*** I continued work on the TO-DO list
***11:56*** I finished the TO-DO list and pushed it to GitHub under the name `Python-TO-DO-list` or just paste the link `https://github.com/NoamSilander/Python-TO-DO-list` (the program is kind of messy but I really don't feel like working on it anymore)

***13:06*** I finalized the list and repo. Taking a break

***Things I learned:***
- `continue` inside a loop stops it, and starts the next round
- You can chain `with` statements (e.g. `with open('file1.txt', encoding='utf-8') as source, open('file2.txt' 'w', encoding='utf-8') as target:)
- the `os` module. At least a part of it. `os.replace('file1.txt', 'file2.txt')` renames `file1.txt` to `file2.txt`, and deletes the origina `file2.txt`
- (almost) All errors are under `Exception`. `OSError` happens when the operating system refuses (or fails) an operation. For example trying to write to a read-only file.
- Main guards: If you have a function/piece of code that runs automatically when the script runs, you should wrap it in a main guard: `if __name__ == '__main__:`. Every Python script has a hidden built-in variable called `__name__`. When the script is run directly, that variable gets assigned the value `__main__`. If the script is imported as a module `import script`, `__name__` gets assigned the script name (without **.py**) as the value. The guard checks if the script is run directly, and only then runs the function/piece of code inside the body. It is done so if you import and use a part of the script in a different script, the automatic parts won't run.

***2.5h spent***

## 04.11.2026
I took a break for today.
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

## 02.11.2026

***Python #3***

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

## 05.11.2026

***Python #5***

***10:48*** I began work on a small login log reporter

***11:30*** I finished v.1 of the login log reporter

***12:50*** I finished v.2 of the login log reporter. It is now way more robust and can actually handle real messy linux logs. I'm quite proud of myself for how it turned out.

***13:07*** I pushed v.2 with a README, under the name `Python-Login-Log-Reporter` or paste the link `https://github.com/NoamSilander/Python-Login-Log-Reporter` Taking a small break

***14:05*** I began work on a word counter

***14:36*** College ended so I'm returning home and taking a break. I got the base of the word counter done.

***Things I learned:***
- `.split()` Takes a string (for example `'My name is John'`) and splits it in the whitespace (if nothing is put into the brackets) and returns a list `['My', 'name', 'is', 'John']`. If something is put inside the brackets (e.g. `.split(',')`), it will split it at the given character e.g. `I,am,not,here` with split(',') will give `['I', 'am', 'not', 'here']`. To limit the amount of cuts you can either use `.split(maxsplit=2)` if you want to split whitespace, or `.split('char', 2)` to stop at 2 splits. `.rsplit` begins the split from the right. `.rsplit(maxsplit=1)` will return the string `My name is John` as `['My name is', 'John]`.
- The `ipaddress` module. I still don't know it fully, but I used it to check for valid IP addresses by trying to assign `ipaddress.ip_address('ip_address')` and seeing if it ValueErrors. If it doesn't, it's a real IP address.

***4h spent***

## 06.11.2026

***Python #6***

***13:37*** I continued work on the word counter

***14:35*** I finished v.1 of the word counter. I tried implementing a sorter function that sorts the numbers in appearance frequency, but I eventually decided to leave it for a later day due to it using complicated logic and new methods and functions I hadn't learned yet. 

***14:43*** I finished writing a README for the counter and pushed it to my GitHub under the name `Python-Word-Counter` or just paste the link `https://github.com/NoamSilander/Python-Word-Counter`. I'm gonna take a break since I don't feel the best right now.

***Things I learned:***
- You can pass lists and dictionaries as parameters in functions
- You can use the `.items()` method on a dictionary to get both the key, and the associated value.
- If you want to remove an item from a list or dictionary you can use the `del` command, to remove it directly, or the `.pop()` method to remove it and pass the removed item to a variable (e.g. `del dict['Key']` or `removed_item = dict.pop('Key')`). You can clear and entire list or dictionary by using the `.clear()` method. 

***1h spent***

## 07.11.2026
I took a break for today.

## 08.11.2026

***Python #7***

***19:50*** I began work on a number guessing game

***22:12*** I finished v.1 of the number guessing game

***22:23*** I finished writing a README for the game, and pushed it to GitHub under the name `Python-Number-Guessing-Game` or just paste the link `https://github.com/NoamSilander/Python-Number-Guessing-Game`

***Things I learned:***
- I previously used the `random` module to shuffle a range using `random.shuffle(list)`. Now I learned `random.radint(x, y)` which will give you a random whole number between the range you gave it. The difference being that unlike in `range(1, 6)` that gives numbers from 1-5, `random.randint(1, 6)` gives a random number from 1-6 (end number included).
- Improved my efficiency and function calling (less unneeded code).

***2.5h spent***

## 09.11.2026

***Python #8***

***12:25*** I began studying JSON files and Python commands in preparation to build a JSON contact book.

***12:48*** I began work on the JSON contact book

***14:36*** I took a break because college ended

***Things I learned:***
- The `json` module. `json.dumps(dict)` takes an existing dictionary, and turns it into a string. While it looks nearly the same, running type() on it will give you `class str`. `json.loads(dict)` does the opposite. it takes the output of `json.dumps()` and turns it back from a string to a dictionary. However, if a dict key is an integer, for example `1`, using `json.dumps()` will turn it into a string `1`. The functions without the `s` at the end are for files and are the way more used ones.
`json.dump(value, file)` and `json.load(file)`.
- Python has `match` cases. you use them by writing ``match name: case 'alice':``, for example. `|` means `or`. `case _:` is the `else` equivalent.
- Type hints. e.g. `def calculator(number1: int, number2: int) -> int:`. 
- You can check if a file exists by using the `os` module using the `.exists()` function of the `path` module. E.g. `os.path.exists('file')`.
- Nevermind `from pathlib import Path` is way better and more modern. you use the searching function by writing `Path(file).exists()`

***2h spent***

## 10.11.2026

***Python #9***

***10:39*** I continued working on the JSON contact book

***12:22*** I made good progress, but I'm taking a small break right now

***12:36*** I continued working

***14:07*** College ended so I'm returning home. I finished implementing adding and saving logic, so i'm really happy with what I've done today.

***Things I learned:***
- `open()` accepts filenames in the `Path(file)` form too.
- The `sys` module. Specifically `sys.exit()` which force closes the program from anywhere.
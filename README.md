# Madlibs-generator
#Accepts a text file as input and displays random line with given madlib by the user.

import random

with open ("madlibs.txt", 'r') as lines:
    line = lines.readlines()
    madlib = random.choice(line)

noun = input("Enter a word:\t")
result = madlib.replace("blank",noun)
print(result)

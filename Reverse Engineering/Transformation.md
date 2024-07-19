#reverse_engineering #_2021_ #completed 
### Description
I wonder what this really is... [enc](https://mercury.picoctf.net/static/0d3145dafdc4fbcf01891912eb6c0968/enc) `''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])`

. . . .
Based on what I think, there is some python, as seen in the question, so its obvious that some knowledge of python is mandatory at this point in order to go further. *But there are other things such as online tools to make things tad bit easier, but not in the long run*

Online Tool - https://www.rapidtables.com/convert/number/hex-to-ascii.html

### Commands used:
#linux_commands **[[LINUX COMMANDS]]** 
1. wget
2. cat

### Steps:
##### Short way:
1. Get the file and *cat* into it to see what's in there. [Looks kind of Japanese's or something]
2. Go to above tool, convert the text into hex and then convert the hex into ASCII.
3. Get the flag and slap it on.
##### Long way:
1. . . .
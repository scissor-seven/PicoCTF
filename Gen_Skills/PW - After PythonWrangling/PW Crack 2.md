#general_skills #_2022_ #completed #picoMini #pass_cracking

# Description
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/13/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) in the same directory too.

# Commands used
#linux_commands  **[[LINUX COMMANDS]]**
1. wget - to download the files `wget [dwnld_lnk_adrs]`
2. python - to run the python script.

# Steps
If you'd ask me, I'd tell you to find multiple methods to solve this one. And not just this, any challenge. It'll give you a perspective to how many ways you can hack into a file or system or such.

Either way, the challenge requires you to read the code, anyway possible.
Read the code, identify that the `user_pw` is provided but in a different format. It's in hexadecimal. If you don't know what that is, go read about it!

It's a string of those, if you concat strings and decode them (or the other way around), you'll get the flag.

- Method 1
 Read those hex codes, put them in any online tool to get their ASCII and shove it as password.

- Method 2
Find a way to mess with the code, and add it in a manner where the provided hex is decoded first, then shows you that `this is the password:...` and you enter it and be done with!

There are all kinds of ways that you can mess with the challenges and widen your own understanding of how these things work!

Enter the password when prompted and you will get your flag.

Next one --> [[PW Crack 3]].
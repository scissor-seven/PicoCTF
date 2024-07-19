#reverse_engineering #_2021_ #completed 

### Description

[crackme.py](https://mercury.picoctf.net/static/be2ba466c6154e42c756bf737ddcecc3/crackme.py)

--> This challenge seems to be twisted at first but get done once observed carefully.

### Commands used
#linux_commands [[LINUX COMMANDS]]
- wget
- python
- nano

### Steps
- Get the files using [[#wget]] onto your webshell.

You can test run the file using [[#python]] command like this ^b6a543

		python crackme.py
This will provide you with test run, try everything.

Look at the source code using [[#nano]] command.

		nano crackme.py
Now observe the whole code very carefully.

If you notice, the `decode_secret()` function is never called, although it has all the decoding code written in it with complete description of about the secret parts of code which are never called.

- At the end, replace the last function call with this -

		decode_secret(bezos_cc_secret)

- Press `ctrl+x` , then `y` , and then press `enter`.
- This will replace the function being called in the code.

Now once you run the code again using -> [[#^b6a543]] , it will reveal the flag instead and the it's done.
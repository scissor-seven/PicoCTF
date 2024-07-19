#general_skills #_2021_ #completed 
### Description

Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/1b247b1631eb377d9392bfa4871b2eb1/ende.py) using [this password](https://mercury.picoctf.net/static/1b247b1631eb377d9392bfa4871b2eb1/pw.txt) to get [the flag](https://mercury.picoctf.net/static/1b247b1631eb377d9392bfa4871b2eb1/flag.txt.en)?

The challenge itself is pretty much clear.

### Commands used:
#linux_commands  **[[LINUX COMMANDS]]**
1. wget
2. python

### Steps:
1. Download all the files on webshell using *wget* command. [ FOR EASE OF PURPOSE, START  MAKING DIRECTORIES OF OF SEPARATE CHALLENGES FOR AN ORGANIZED WORKFLOW]
2. *cat* the pw.txt file before hand to get the password for python file.
3. To run the python file to 'd'ecode the *flat.txt.en*  encrypted file, the syntax is

		python ende.py -d flag.txt.en
	- In the above command-
		- python or python3 [depending on environment] is mandatory to run any python script.
		- then comes the python_filename
		- then there is option [-d in our case to decrypt]
		- then the enc_filename
		[ All the filenames must be used with their EXTENTIONS. If in other directory, then with their FULL ADDRESS & EXTENSIONS ]
4. copy-paste the flag and done.	
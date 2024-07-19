#reverse_engineering #_2021_ #completed 

### Description
[keygenme-trial.py](https://mercury.picoctf.net/static/b016c61bd2cc0be05a59da1dde67a2ac/keygenme-trial.py)

Nothing more is there in question but from what I can tell, looking at the code, the flag has 2 parts. One is static meaning it stays the same, other is dynamic meaning it changes every time we run the code.
For dynamic part, we see that what its doing is taking *username_trial*, hashing it using SHA256 algorithm, and after getting the hash, its taking certain *indexes*, from that hash, concatenating them, thus getting the *key*

### Commands used
#linux_commands [[LINUX COMMANDS]]
- wget
- nano
- python

### Steps
1. Get the file.
	- FOR THIS LAB, I RECOMMEND TO KEEP A NOTEPAD/TEXT EDITOR OPEN.
2. Run the file, see all kinds of responses.
3. Once done go check the code using this command

		nano keygenme.py
4. Doing so opens the source code in *nano* editor.
	 - If you understand the code somewhat, you'll see that the flag has a static part, which is fixed and last part is dynamic, which changes based SHA256 HEX hashing of the *b'Username_trial'* variable. And within the whole hash, there are certain indexed being used for the last part of the key.
5. From the source code, note what algorithm is being used to hash, what IS being hashed, and what indexes from hash are being used for the dynamic part of FLAG.
6. Run the following commands in sequence:

		python
	This command will open a python interpreter, which will look like `>>>` this.

		hash = hashlib.sha256(b'GOUGH').hexdigest()
	The username variable in our case is GOUGH. `You can know yours if you run the keygenme.py` file.

	If you want to see your hash, you can do this

		print(hash)
	At this `>>>` point in you terminal.
7. After looking at the whole hash, you have to concatenate the indexes that you have noted by doing this

		hash[4]+hash[5]+hash[3]+hash[6]+hash[2]+hash[7]+hash[1]+hash[8]
	This will show you your `dynamic` part of the flag.
8. Once done, JOIN both the parts of flag, STATIC and DYNAMIC & SUBMIT
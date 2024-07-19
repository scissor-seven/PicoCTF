#general_skills #_2021_ #completed 
### Description

Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/a00f554b16385d9970dae424f66ee1ab/warm) has extraordinarily helpful information...

For this challenge, I suggest beginners must go through all the hints for a good understanding. This one is pretty much follow the steps precisely.

### Commands used:
#linux_commands **[[LINUX COMMANDS]]**
1. wget
2. **./** - this ones more like something to use to run an executable file
3. chmod

### Steps:
1. Get the files.
2.  Use chmod command to change/modify the property of the file.

		chmod +x warm
	- In the above command-
		- *chmod* keyword to invoke it
		- *+x* to add the property of making the file executable
		- *file_name* at the last
3. Execute the file-

		./warm
1. As the output suggests, use -h with the *file execution* command

		./warm -h
1. Viola, you get answer, slap it on the box and submit.
#general_skills #_2021_ #completed 

### Description
Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/ff4e569d6b49b92d090796d4631a2577/static)? This [BASH script](https://mercury.picoctf.net/static/ff4e569d6b49b92d090796d4631a2577/ltdis.sh) might help!


### Commands used
#linux_commands [[LINUX COMMANDS]]
1. wget
2. cat - to view the file contents in raw, possible textual format
3. grep - to search for specific term, phrase or process in a file.

IN OUR CASE, THE OUTPUT OF *CAT* COMMAND IS BEING PIPED TO GREP USING " | " OPERATOR. 

### Steps
Get the files using wget command

You can *cat* the static file but won't get to any conclusion. Try running the `ltdis.sh` script but it won't allow so give it permission using the command given below.

	chmod +x ltdis.sh

Now try to run the script with below command and it'll probably show some error.

	./ltdis.sh
What you can try though is this command

	./ltdis.sh static
The point is, if you read carefully the error with ONLY script command is that it needs and input file in order fully execute, which we provide in previous command.

Doing so gives us **2 txt** files. You can *cat* both files, but the **x86** file has some hex code and *strings* file is too long.

You can use this command to search for the flag in both file

	cat static.ltdis.strings.txt | grep pico

&

	cat static.ltdis.x86_64.txt | grep pico

Whichever gives flag, submit it, thus solved!!!
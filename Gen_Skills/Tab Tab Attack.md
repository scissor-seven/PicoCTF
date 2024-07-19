#general_skills #_2021_ #completed 

### Description

Using tab-complete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames: [Addadshashanammu.zip](https://mercury.picoctf.net/static/3afd18a65e42b80526aa87f9766c588b/Addadshashanammu.zip)

This lab is pretty straight forward, if you are familiar with some common commands.

### Commands used
#linux_commands [[LINUX COMMANDS]]
-  wget
-  unzip
- ls
- exiftool

### Steps
1. Get zip file using wget and the URL from [[#Description]].
2. Unzip the file using following command

		unzip Addadshashnammu.zip
	- This command by default unzips a zip file, without passing any option.
3. Once done, type

		cd Addadshashnammu
And then keep pressing TAB key until the command stop by itself.

4. Once in the directory, type

		ls
To list the directory contents
5. You'll find there is a file. You can check its data using `exiftool` command

		exiftool fang-of-heynekhtnamet
Showing us its an executable file
6. Enter

		./fang-of-haynekhtnamet
To execute and there is your FLAG.
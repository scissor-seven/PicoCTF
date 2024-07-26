#general_skills #_2022_ #completed #picoMini #pass_cracking

# Description
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/11/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/11/level1.flag.txt.enc) in the same directory too.

# Commands used
#linux_commands  **[[LINUX COMMANDS]]**
1. wget - to download the files `wget [dwnld_lnk_adrs]`
2. python - to run the python script.

# Steps
Compared to previous one, [[Python Wrangling]], this one requires the attention on code and understand. Either you know how to code, which would make it easy for you to read. If not, just punch the code in any AI and ask it what it to explain. That'll do.

As far as the challenge itself, if you read the code, you know the password. It is clearly pretty clear!

Run the python script on shell:
```shell
python .\level1.py .\level1.flag.txt.enc
```
Enter the password when prompted and you will get your flag.

Next one --> [[PW Crack 2]].
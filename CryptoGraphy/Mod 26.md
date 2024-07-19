#cryptography  #_2021_ #completed 
### Description

Cryptography can be easy, do you know what ROT13 is? (link on next line)

This challenge presents with a problem of decryption of file using certain decryption algorithm, **[[ROT13]]** in our case. It can be solved multiple ways. If you read the hint, it states that it can simply be done online or through the CLI.

### Commands used:
#linux_commands  **[[LINUX COMMANDS]]**
1. echo
2. pipe ( | ) - its not like a command, its more so like an operator.

### Steps:
#### a. Online method
1. Simply copy the text encoded.
2. Go to an online [[ROT13]] decoder
3. Get the flag & submit.

#### b. CLI method
NOTE : Only in case of [[ROT13]], if the encrypted code is re-encrypted, and output is the plaintext.
1. Run *echo* command followed by the encrypted message in "double quotes".
2. On the same line, after message, ***pipe*( '|' )** the command to -  *tr 'A-Za-z' 'N-ZA-Mn-za-m' 
3. the command should look somewhat like this
	echo "asdad ouerqk" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
# Secret-Codes
Assignment done in my Honors CS Class


Directions

Your goal is to write a program that will take a word from the user and encrypt it using various encryption options that the user will specify. First, some context…

Cryptography is the process of modifying/scrambling/changing messages so that they can be transmitted securely over computer networks. Computers encode and decode information often as precious data is sent across the big, bad internet. There are various methods of encryption known as “cyphers.” There are various types of cyphers - even some that have existed for thousands of years! In this problem we will use various shift and circle cyphers, which will involve shifting letters around in a word in order to encrypt it.  

The program will take a single line of input from the user, which will contain both encryption commands and the word the user wants to encrypt. The following format will be used for data entry:

COMMAND1-details/COMMAND2-details/.../COMMANDX-details/messageToEncrypt

The user will enter a series of commands, with each command ending with a forward slash character (/). The name of the command will be entered, followed by a dash character(-), and then the details/arguments for that command will be entered. Each command will use a specified number of numerical arguments. The user should be able to enter any number of commands. To end the input, the user will enter the word that they want to encrypt using the entered commands. 


See the command descriptions and sample runs / test data on the following page!


Available Commands

LS-X: Shifts all the characters of the string X places to the left. The leftmost X characters are deleted and X #’s are inserted on the right to return the string to its original length. LS–3 COMPUTER = PUTER###
 
RS–X: Shifts all the characters of the string X places to the right. The rightmost X characters are deleted and X #’s are 
inserted on the left to return the string to its original length. 

Example: RS–3 COMPUTER → ###COMPU
 
LC-X: Circulates the leftmost X characters to the right-hand side of the string. 

Example: LC–3 COMPUTER → PUTERCOM
 
RC–X: Circulates the rightmost X characters to the left-hand side of the string. 

Example: RC–3 COMPUTER → TERCOMPU
 
MC–SLXD: Circulates the sub-string starting at position S, with a length of L, X characters, in direction D (Left or Right). Each argument (S, L, X and D will be one character in length. The direction D will be either L for Left, or R for Right.

Example: MC–332R COMPUTER → COPUMTER
 
REV–SL: Reverses the order of the characters starting at position S with a length of L. 

Example: REV–33 COMPUTER → COUPMTER

Example Runs / Test Data

Input: 	LS-1/RS-1/OHIO
Output: 	#HIO
Input: 	LS-1/LC-3/MC-453L/MEMORIAL  
Output: 	RIAMOL#E
Input: 	RC-2/LC-5/CINCINNATI 
Output: 	CINNATICIN





Codebreaker

Code breaking is all about finding the secret code.

Your mission is no different!

Using test driven techniques, you have to implement a simple program that fulfill the basic following requirements:

When the game starts I should be able to guess the secret code by providing a 4 digits number
The game finishes when I have found the exact match for the secret code
The game will return a + sign for an exact match
The game will return a - sign for a digit match
An exact match is a digit that matches a digit of the secret code both in value and in position
A digit match is a digit that matches a digit of the secret code in value but does not have the correct position
Example: Let us say the secret code is 1234. 
         If you provide 1245 the program should 
         return the string '++-' indicating 
         two exact matches (1,2) and one digit match (4)

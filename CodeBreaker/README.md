#Codebreaker

Code breaking is all about finding the secret code.

Your mission is no different!

Using test driven techniques, you have to implement a simple program that fulfill the basic following requirements:

When the game starts I should be able to guess the secret code by providing a 4 digits number
The game finishes when I have found the exact match for the secret code

1. The game will return a + sign for an exact match
2. The game will return a - sign for a digit match
3. An exact match is a digit that matches a digit of the secret code both in value and in position
4. A digit match is a digit that matches a digit of the secret code in value but does not have the correct position
5. Exact matches have priority over digit matches
6. Once a digit has been matched, either exactly or just digit match, in the **secret code**, it can no longer be used for another match


Examples: 

Secret: 1234, Proposal: 1245 --> Response: '++-' because two exact matches (1,2) and one digit match (4)

Secret: 1234, Proposal: 2002 --> Response: '-' 

Secret: 1234, Proposal: 2200 --> Response: '+' 

Secret: 1100, Proposal: 1010 --> Response: '+' because 1 has been used to match the first digit in the secret and can no longer be used to match the second 1. Rule 6

Secret: 1100, Proposal: 0011 --> Response: '-' because 1 has been used to match a digit and can no longer be used. Rule 6

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
6. Once a digit has been used for an **exact match** in the **secret code**, it can no longer be used for any **digit match**


Examples: 

Secret: 1234, Proposal: 1245 --> Response: '++-' because two exact matches (1,2) and one digit match (4)

Secret: 1234, Proposal: 2002 --> Response: '-' because 2 has been used once for a digit match, cannot be re-used (rule 6) 

Secret: 1234, Proposal: 2200 --> Response: '+' 

Secret: 1234, Proposal: 1234 --> Response: '++++'

Secret: 2234, Proposal: 2234 --> Response: '++++'

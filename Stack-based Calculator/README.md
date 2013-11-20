# Stack-based arithmetic calculator

Create an stack-based arithmetic calculator. Print out in the console the intermediate state of the stack

* Inputs = list of operands, list of operations
* Output = result of the operation

To simplify the exercice, we only consider the 4 basics *2-operands* operations: +, -, *, / 

Example:

Input = **[3,2,5], [\*,+]**

Display:

* **[3,2,5], [\*,+]**
* **[3,7], [\*]**
* **[21], []**

Ouput = **21**

Explanation:

1. **[3,2,5], [\*,+]**  (pop operation +, pop 5 and 2, 5+2=7, push back 7 to the stack)
1. **[3,7], [\*]**  (pop operation \*, pop 7 and 3, 7\*3= 21, push 21 back to the stack)
2. **[21], []** 
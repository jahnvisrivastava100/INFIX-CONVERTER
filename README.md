## INFIX-CONVERTER

# USE
converts an infix expression to postfix or prefix as per users choice.

# Convert Infix to Postfix Notation

Initially we have an expression exp which represent the expression in infix format. Now we need a character stack.

We will iterate through the string exp, from left to right.

Whenever we encounter an operand we’ll add it to are character array post[].

If we encounter an ‘(‘ we’ll push it to the stack.

If we encounter an ‘)’ we’ll take the following actions:

We’ll continue to pop top of the stack until we find the ’(‘
Before we pop top of the stack, we’ll enter every character of top of the stack into string post except ‘)’   (  ')' will be discarded).
If we encounter an operator, we’ll take the following actions:

We’ll continue to pop top of the stack s until we find that exp[i] is greater than the top of the Stack  s(by the rules of precedence for which two functions are made to specify precedence) 
When the traversal will be finished, we’ll continue to pop top of the stack and keep on adding in our char array post[]   until stack is  empty.

# Convert Infix to Prefix Notation
Initially we will take  a string exp from user which represent the expression in infix format.

Reverse the string exp. After reversing (for Eg. A+B*C will become C*B+A. )Note while reversing each ‘(‘ will become ‘)’ and each ‘)’ becomes ‘(‘.

Obtain the postfix expression of the modified string exp. We have to handle the ‘(‘ as ‘)’ and ‘)’ as ‘(‘

Just reverse the postfix expression we wil get our desired prefix expression
# check
here check function checks for validity of the expression and allows conversion only when entered expression is valid

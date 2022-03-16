# lab report 5 week 10
I found test with different results by searching through manually

# test 1 - 498.md
my implementation output:
![image](Screenshot (176).png)
provided implementation output:
![image](Screenshot (175).png)

Both implementations are not correct, 
the expected output would be a link in the configuration of foo(and(bar), [foo(and(bar)]. 
## bug in code
The part that is wrong in my implementation is that is takes in the whole content within the first open parenthesis and first close parenthesis,
while in fact it should omit the the < sign and > sign and include the content up to the outermost close parenthesis. 
## code to be fixed
![image](Screenshot (184).png)
The fix about my implementation would be to add two fields in the while loop called lessThanSign and largerThanSign, 
and to have them equal to the index of < and > sign, and if both variables != -1, then have the toReturn add a subtring within < and > signs.

# test 2 - 496.md
my implementation output:
![image](Screenshot (181).png)
provided implementation output:
![image](Screenshot (180).png)

The provided implementaions is correct, my implementation is wrong. 
This is not a valid link, so the expected output would be empty in the brackets, [].
## bug in code
The part that is wrong in my implementation is that it takes in the content within the first open parenthesis and first close parenthesis,
while in fact it shouldn't take in anything between the outermost open parenthesis and outermost close parenthesis,
as the number of open and close parentheses between them do not match, 
within the outermost open parenthesis and outermost close parenthesis, 
there are 2 open parentheses and 1 close parenrthesis. 
## code to be fixed
![image](Screenshot (183).png)
The fix about my implementation would be to add 2 counters in the method to count the number of open and close parentheses respectively, 
and have the toReturn add susbtrings only when counter1 matches counter2 with an if statement. 

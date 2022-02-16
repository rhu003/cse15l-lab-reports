# week 4 lab report

## Change 1
![image](Screenshot (97).png)
test file: test file2.md
[Link](https://github.com/rhu003/markdown-parse/blob/main/test-file2.md)

Sympton by showing command and output: 
![image](Screenshot (84).png)

The sympton was it runs an infinite loop. This is caused by a bug in MarkdownParse.java that it didn't exit the while loop properly.
As we can see in input file test-file2.md, the last line is not a valid link, so nextOpenBracket, nextCloseBracket, openParen, closeParen would be -1. 
In order to have it exit the while loop properly, we need to break the loop based on the condition of last line in test-file2.  

## Change 2
![image](Screenshot (100).png)
test file: test-file3.md
[Link](https://github.com/rhu003/markdown-parse/blob/main/test-file3.md)

Sympton by showing command and output: 
![image](Screenshot (87).png)

The sympton was string index goes out of bounds. This is caused by a bug in MarkdownParse.java when the openParen can't be found in test-file3. 
As we can see in input file test-file3.md, line 3 has open and close brackets, but not open and close parentheses.
So we can simply have the loop exit when openParen becomes -1. 

## Change 3
![image](Screenshot (102).png)
test file: test-file4.md
[Link](https://github.com/rhu003/markdown-parse/blob/main/test-file4.md)

Sympton by showing command and output: 
![image](Screenshot (104).png)

The sympton was string index goes out of bounds. This is caused by a bug in MarkdownParse.java when closeParen can't be found in line 4 of test-file4.
As we can see in input file test-file4.md, line 4 has open parenthesis, but not closed parenthesis.
So we can simply have the loop exit when either one of openParen or closeParen equals -1.

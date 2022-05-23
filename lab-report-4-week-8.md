# Lab Report 4
- [my markdown-parse repo](https://github.com/aejiang/markdown-parser)
- [repo reviewed in week 7](https://github.com/Miyuki-L/markdown-parser)

**Snippet 1**
- what should be produced: ``[`google.com, google.com, ucsd.edu]`` based on VScode Preview

- This is a screenshot of my test for snippet 1.
![image](https://user-images.githubusercontent.com/103210217/169721027-a6d46eb3-5954-4b1d-9993-adc912334236.png)

- The test did not pass for my implementation. Here is the test failure.
![image](https://user-images.githubusercontent.com/103210217/169720927-ab245a97-97f1-40c5-9602-01d7fd1137fd.png)

- The test also did not pass for the implementation I reviewed in week 7. Here is a screenshot of the test failure.
![image](https://user-images.githubusercontent.com/103210217/169721116-0801b338-3f76-444b-95e2-5524414a3c76.png)

**Snippet 2**
- what should be produced: ``[a.com, a.com(()), example.com]``

- This is a screenshot of my test for snippet 2.
![image](https://user-images.githubusercontent.com/103210217/169721476-05efa2d5-3aeb-4e1b-bab5-5252cce7e100.png)


- The test did not pass for my implementation. Here is a screenshot of the test failure.
![image](https://user-images.githubusercontent.com/103210217/169721503-23874422-8419-4db6-8db4-77d2d1f3f3f9.png)


- The test also did not pass for the implementation I reviewed in week 7. Here is a screenshot of the test failure. 
![image](https://user-images.githubusercontent.com/103210217/169721553-1bf52255-2d7f-4202-972f-16bda81c6df4.png)



**Snippet 3**
- what should be produced: ``[https://www.twitter.com, https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule, https://cse.ucsd.edu/]``

- This is a screenshot of my test for snippet 3.
![image](https://user-images.githubusercontent.com/103210217/169722667-5c0a1e27-9719-44ba-9889-287812ef2cc5.png)

- The test did not pass for my implementation. Here is a screenshot of the test failure.
![image](https://user-images.githubusercontent.com/103210217/169722642-319f07d2-136c-4d35-83be-9d78ee8f1a8d.png)

- The test also did not pass for the implementation I reviewed in week 7. Here is a screenshot of the test failure. 
![image](https://user-images.githubusercontent.com/103210217/169722713-aece9473-f841-46d8-b8d3-027eb801abf6.png)

**Questions**
- Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.
```
Yes, I do think a small code change will make my program work for snippet 1. For this code change, I would check for a pair of backticks and parentheses or brackets within the backticks. If these characters are in the backticks, then they don't count as a valid open/ close parentheses/ bracket variable.
```
- Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.
``` 
Yes, I do think there is a small code change that will make my program work for snippet 2. I would use a stack to group pairs of parentheses and brackets, to avoid closing off a link too early. 

- Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.

No, I do not this there is a small code change that will make my program work for snippet 3. I think a more involved change is needed because my current code only checks for parentheses and brackets for each line. The link text and url's go beyond a single line, so the program essentially starts fresh each line and isn't able to correctly find the link text and url's. I would have to change the structure of my code to not only check line by line.



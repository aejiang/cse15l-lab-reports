# Lab Report 5

**How I found the tests with different results**
I found the tests by running the time bash command for both markdown parsers. Then I manually compared the outputs from each until I found differences.
**Links to the test files with different results
- [test1](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/32.md)
- [test2](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/371.md)

**Test 1**
- Describe which implementation is correct or neither:
```
My implementation on the left is correct because it correctly prints out the title of the link whereas the other implementation prints out an empty array.
```
- Screenshots of both outputs and the expected outputs:
![test1](https://cdn.discordapp.com/attachments/983267884333670450/983269097062146118/unknown.png)
- This is a screenshot of the outputs of both implementations for test 1.

![exp1](https://user-images.githubusercontent.com/103210217/172124386-bc570337-d0ff-4f9a-8288-40fadf107120.png)
- This is a screenshot that shows that `[/f&ouml;&ouml; "f&ouml;&ouml;"]` should be the correct output according to commonmark.

**Test 2**
- Describe which implementation is correct or neither 
```
The implementation on the right is correct. It correctly outputs the empty array because there is no valid link in the file.
```
- Screenshots of both outputs and the expected outputs 
![test2](https://media.discordapp.net/attachments/983267884333670450/983269300716589146/unknown.png)
- This is a screenshot of the outputs of both implementations for test 2.

![exp2](https://user-images.githubusercontent.com/103210217/172125652-b31172d3-e481-417d-b994-6e895ba97d04.png)
- This is a screenshot that shows that the empty array should be the correct output according to commonmark.

- for wrong implementation, describe bug in 2-3 sentences (what is wrong and code that should be fixed) (ss of code highlighting what should be fixed)

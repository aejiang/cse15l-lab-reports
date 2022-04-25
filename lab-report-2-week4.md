# Lab Report 2

**Code Change 1**
![change1](https://user-images.githubusercontent.com/103210217/165003380-0198c2ee-bd1a-4ee4-9b29-2709e2b7760d.png)
- [This](https://github.com/aejiang/markdown-parser/blob/main/test-file-link-mid.md) is test file 1 for the error caused by putting a link in the middle of the file.
![symptom1](https://user-images.githubusercontent.com/103210217/165024258-e4c70434-3959-443b-83e8-8bf5e7935b1f.png)

- The first bug is that the program cannot does not know to move to the next line when there is no link in that line. A symptom is seen in the terminal after running it with a file with 2 links in the middle of empty lines. It runs into an OutOfMemoryError because the while loop runs forever, but it should print out the two links in the file. 


**Code Change 2**
![change2.1](https://user-images.githubusercontent.com/103210217/165023263-7832e19b-52e9-4c86-905b-be46f70e6643.png)
![change2.2](https://user-images.githubusercontent.com/103210217/165023304-2d895e06-fe52-4f66-9c17-c9dfc12b952a.png)
- [This](https://github.com/aejiang/markdown-parser/blob/main/test-file-Img.md) is test file 2 for the error of getting links of images. 
![symptom2](https://user-images.githubusercontent.com/103210217/165022847-e0d1f905-3c34-4a9d-8132-dfb93d890d48.png)

- The second bug is that the program prints out image links when it's not supposed it. The symptom of this is seen in the output after running on a file with an image link and url. The output includes the image link and the url, but it should only include the url.  



**Code Change 3**
![change3](https://user-images.githubusercontent.com/103210217/165025715-b34e79be-111a-4013-8ca8-9b01836866ec.png)
- [This](https://github.com/aejiang/markdown-parser/blob/main/test-file-onlyBrackets.md) is test file 3 for the error caused by having only brackets.
![symptom3](https://user-images.githubusercontent.com/103210217/165025172-a2f05617-3e67-4951-86f4-536a24f7d8e2.png)

- The third bug is that the program does not work properly on files with only brackets and no parentheses. A symptom is seen in the terminal after running the program on a file with only brackets in one line and a url in another. After running, a StringIndexOutOfBoundsException shows up because the index of the open and closed paretheses cannot be found. 

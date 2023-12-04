## Student's Post
Hi, I was curious why I keep getting this error message. I tried testing the `ListExamples.java` and `ListExamplesTests.java` file using `bash test.sh` command, but it keeps generating the `TestTimedOutException` error indicating the error occured at line 44 in the `merge` method of `ListExamples.java` and in the line 19 `testMerge2` method of `ListExamplesTests.java`. Could you help me fix these errors? I uploaded both the `merge` and `testMerge2` class. 

![image](bashfail.png)

![image](mergemethodfail.png)

![image](test2mergefail.png)

I am uploading the whole code of `ListExamples.java`, just in case the error is being generated in other areas.

![image](listexamplesjava.png)

## TA's Response
Hi there, the reason you're getting error messages is because you labelled the variable wrong in the `merge` method in `ListExamples.java`. Notice that the `merge` method in `ListExamples.java` aims to take two sorted list of strings and return a new list hat has all the strings in both list in sorted order. Replace `index1` in line 43 with a suitable variable that aligns with other variables in the third `while` method. Hint: the third while loop checks if the index reached at the end of `list2`, not `list1`.

Also, I noticed in your `filter` method in `ListExamples.java`, your code result.add(s) appends a new string `s` at the beginning of the string `result`. This does not match the description of the `filter` method. Your code prints out the reversed version of the expected output. Make a modification in line 15 so that it prints out `result` in correct order.

## Follow-up by studetn
![image](bashpassed.png)

![image](dnjn.png)

![image](.png)

![image](dnjn.png)

![image](listexamplesjava.png)



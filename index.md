Ryan Ryu - CSE 15L Lab1 Report
---
Hi everyone, this is Ryan and today I'm going to be talking about a few commands to use in terminal: *cd*, *ls*, and *cat*.
In this specific blog post, we're gonna be looking at this simple file structure.

![image](Screen Shot 2023-10-09 at 11.32.58 AM.png)

---
# `cd (Change Directory)` switches the current working directory to the given path.
## 1) When it is used with no arguments,
   - It defaults to the home directory, which in this case is */home*.
     ![image](Screen Shot 2023-10-09 at 11.32.20 AM.png)
   - As you can see in the picture, the working directory was */home/lecture1* when the command was run, but it defaulted to */home* when *cd* was run without arguments.
   - This is because when *cd* is used without arguments, it indicates to the terminal that it wants to redirect to home directory.
   - Using *cd* without arguments do not generate an error. 
  
## 2) When it is used with a path to directory as an argument,
   - It redirects the working directory to the directory that is used as the arguement.
     ![image](Screen Shot 2023-10-09 at 11.50.53 AM.png)
   - In this case, the working directory was /home. But when it is redirectred to the path *./lecture1*, it swtiches the working directory to */home/lecture1*
  
## 3) When it is used with a path to file as an argumemt,
   - It generates an error.
     ![image](Screen Shot 2023-10-09 at 11.54.43 AM.png)
   - The working directory was /home/lecture1/messages. When it is redirected to a file using *cd ./af.txt*, it generated an error.
   - This is because cd only changes to 'directories', but the file.
   - Thus, it generates an error noting that *af.txt* is 'Not a directory'.

---
# `ls (List)` lists the files and folders in the given path.
## 1) When it is used with no arguments,
   - It lists the items in the given path.
     ![iamge](Screen Shot 2023-10-09 at 12.06.38 PM.png)
   - In this case, it listed each text file in the */messages* directory.
   - The working directory was */home/lecture1/messages*, and it remained the same throughout the command. It only lists the files and folders in this directory and does not change the directory.
   - It does not generate an error.
   
## 2) When it is used with a path to directory as an argument,
   - It shows the items in that directory.
     ![iamge](Screen Shot 2023-10-09 at 12.10.36 PM.png)
   - In this image, it shows the items in the */home* directory.
   - the working directory was */home*, and it stays the same after the command.
   - This output was generated because ls command lists the items in a given path.
   - It does not generate an error.
   
## 3) When it is used with a path to file as an argumemt,
   - It just restates the path to the file.
     ![iamge](Screen Shot 2023-10-09 at 12.18.03 PM.png)
   - In this image, it only shows the path to the exact file that was used as the argument, which is */home/lecture1/messages/af.txt*.
   - The working directory stayed the same throughout the command.
   - I got this output because you cannot list the files inside a file. There is only one item to be displayed, which is the file itself.
   - It does not generate an error. It lists out the file in the given path.

---  
# `cat (Concatenate)` prints the contents of one or more files provided by the paths
## 1) When it is used with no arguments,
   - It duplicates your input until you exit by pressing Ctrl + D.
     ![iamge](Screen Shot 2023-10-17 at 7.26.29 PM.png)
   - It duplicated 'it' and 'duplicates' which I typed in.
   - It does this because it is instructed to print out my input.
   - The working directory remains the same. (Working directory: */home*)
   - It does not generate an error.

## 2) When it is used with a path to directory as an argument,
   - It states whether the given path is a directory or not. 
     ![iamge](Screen Shot 2023-10-09 at 12.37.28 PM.png)
   - In this example, it says *./messages* is a directory.
   - The working directory still stays */home/lecture1*.
   - I got this output because for directories, it displays whether or not it is a directory.
   - It generates an error because `cat` cannot concatenate the contents of a directory.
   
## 3) When it is used with a path to file as an argumemt,
   - It shows the contents of the given file used as arguments.
     ![iamge](Screen Shot 2023-10-17 at 7.35.56 PM.png)
   - It printed out the contents of both *Hello.java* and *README*.
   - The working directory did not change. (Working directory: */home/lecture1*)
   - *cat* printed out the contents, because files are used as arguments.
   - It does not generate an error.

### Disclaimer: When I tried to save this webpage as a PDF file, it did not show the box around the words like `cd`,`ls`, and `cat` when used with with ` (backticks). However, when you visit the webpage [https://ryanryucode.github.io/cse15l-lab-reports/](https://ryanryucode.github.io/cse15l-lab-reports/) it displays the words in boxes when used with backticks.

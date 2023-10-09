Ryan Ryu - CSE 15L Lab1 Report

Hi everyone, this is Ryan and today I'm going to be talking about a few commands to use in terminal: cd, ls, and cat.
In this specific blog post, we're gonna be looking at this simple file structure

![image](Screen Shot 2023-10-09 at 11.32.58 AM.png)

cd (Change Directory) switches the current working direcetory to the given path
1) When it is used with no arguments,
   - it defaults to the root directory, which in this case is */home*
   - (pic)
   - As you can see in the picture, the working directory was /home/lecture1 when the command was run, but it defaulted to /home when cd was run without arguments
   - This is because when cd is used without arguments, it indicates to the terminal that it wants to redirect to home directory
   - Using cd without arguments do not generate an eroor. 
  
2) When it is used with a path to directory as an argument,
   - it redirects the working directory to the directory that is used as the arguement
   - (pic)
   - In this case, the working directory was /home. But when it is redirectred to the path ./lecture1, it swtiches the working directory to /home/lecture1
  
3) When it is used with a path to file as an argumemt,
   - It generates an error.
   - (pic)
   - The working directory was /home/lecture1/messages. When it is redirected to a file using cd ./af.txt, it generated an error.
   - This is because cd only changes to 'directories', but the file.
   - Thus, it generates an error noting that af.txt is 'Not a directory'
  
<ls>
- path to file as an argumemt
  -> screenshot of command & output
  -> working directory
  -> why I got this output
  -> if it's error/not, why/not
<cat>


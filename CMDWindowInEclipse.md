# How to open a Windows Command Prompt in my console in Eclipse

There are a few ways to do it, but a simpler way is to use the "external tools configuration". In a few steps, you can have a command prompt (DOS Windows) at the console in Eclipse. 

For detail, refer to the following: http://www.avajava.com/tutorials/lessons/how-do-i-open-a-windows-command-prompt-in-my-console.html.

1. Click the 'External Tools Configuration' option on the <Run> <External Tools> menu. 
2. Click the 'New Launch Configuration' button (with + sign) to create a new External Tool configuration. 
3. Name this configuration 'Command Prompt' instead of the default "New Configuration" at the top of the form.
4. Click the 'Browse File System...' button to select the location of 'cmd.exe' (C:\WINDOWS\system32\cmd.exe). 
5. Click the 'Browse File System...' button to set the Working Directory to , for example, 'C:\users\user' so that the Command Prompt will start at C:\users\user. 
6. Click the 'Apply' button. 
7. 
    

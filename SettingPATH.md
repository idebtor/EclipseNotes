# How to udpate the PATH environment variable

The following explains how to update the PATH environment variable.
### in Windows 7 or 8. 

After installing Java SE Development Platform, we must update the PATH environment variable to include Java path. The PATH environment variable is a series of directories separated by semicolons (;). Microsoft Windows looks for programs in the PATH directories in order, from left to right. You should have only one bin directory for the JDK in the path, you just update that particular entry.

The following is an example of a PATH environment variable:
```
C:\Program Files\Java\jdk1.8.0_65\bin;C:\ProgramData\Oracle\Java\javapath;C:\Program Files (x86)\Intel\iCLS Client\;C:
```
From the desktop, right click the Computer icon.
  1. Choose Properties from the context menu.   
  2. Click the Advanced System Settings link.
  3. Click Environment Variables. In the section System Variables, find the PATH environment variable and select it. Click Edit.
  4. In the Edit System Variable window, specify the value of the PATH environment variable. Click OK. 
   **Note**: Not to misspell the path name, you may use the window file explorer to locate java bin folder.
    Then click the path name to select at the top of the explorer. Copy the path.)
  5. Close all remaining windows by clicking OK.

To verify that the path is set by calling a java command:
  1. Bring up a console window by entering cmd or powershell 
   (by clicking Start button, and type cmd or powershell in command window.)
  2. Enter a java command such as:
  
```
java -version
javac -version
```

### in Linux
To set the path permanently, set it in your shell startup file.

For C shell (csh), edit the startup file (~/.cshrc):
```
set path=(C:\Program Files\Java\jdk1.8.0_65\bin $path)
```

For bash and ksh, edit the startup file (~/.bashrc):
```
PATH=C:\Program Files\Java\jdk1.8.0_65\bin:$PATH
export PATH
```

For sh, edit the profile file (~/.profile):
```
PATH=C:\Program Files\Java\jdk1.8.0_65\bin:$PATH
export PATH
```

Then load the startup file and verify that the path is set by repeating the java command:
For C shell (csh):
```
% source ~/.cshrc
% java -version
```
For ksh, bash, or sh:
```
% . /.profile
% java -version
```

# How to set CLASSPATH
Classpath in Java is path to directory or list of directory which is used by ClassLoaders to find and load class in Java program.

For CLASSPATH, refer to [How to set CLASSPATH for Java on Windows and Linux](http://javarevisited.blogspot.kr/2011/01/how-classpath-work-in-java.html)



# A better way to add .jar files in Eclipse

There are a few ways to java library files to include in Eclipse. A better way is to add the jar to build path so your project will compile if exported:

    - Step 1. Create a folder called lib in your project folder.
    - Setp 2. Copy or move to this folder all the jar files you need. 
                You may even move all the source code to build them.
    - Step 3. Select <Refresh> to refesh your project in <File> menu. 
                Then the folder lib you created in Step 1 is listed in Package Explorer.
    - Step 4. Select all the jar files, then right click on one of them and select Build Path -> Add to Build Path

Then you will see your library files listed automatically under Referenced Libraries of Package Explorer
  
**Note**: Adding external Jar is not smart in case you want to change the project location in filesystem. The following steps are **not** recommended since it includes a **hard-wired** path name. 
```
  Eclipse -> Preferences -> Java -> Build Path -> User Libraries -> New(Name it) -> Add external Jars
```
  

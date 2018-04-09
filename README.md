# cesm2cases
This README is for storing your case in your own git repository for.  It is a light weight way
for the cesm experimentor to keep track of cases.

1. Create a cesm2cases fork on github - you only need to do this once.   You are forking the
    repository at https://github.com/jedwards4b/cesm2cases
2. clone your fork to the hpc filesystem where your case is located
3. Use the following script to copy files from the clone to your case directory
    ```
    cp clone/.gitignore case/
    cp -r clone/.git case/
    cp clone/README.md case/
    ```
4. go to your case directory and run git status, this will give you
    the list of files you should add from your case to the repository

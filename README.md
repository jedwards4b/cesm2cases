# cesm2cases

This repository is a template for storing your cesm2 case using git.
It is a lightweight way for the cesm experimentor to keep track of cases.

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
    the list of files you should add from your case to the repository.

5. Create a branch for this case in your git repo and add the files you want to save.
    In particular you should add the user_nl files, any files under
    SourceMods, and all *.xml files.

6. commit and push these changes to your remote branch.
# Create a Python Virtual Environment (venv) in VSCode

Useful video explaining the process:
https://www.youtube.com/watch?v=8h9w0meM8i4&t=308s


A venv consists of an interpreter and packages. The purpose of having and using venv's is to keep certain packages seperated. For example, script-A might run package-X (v1.0), while script-B might run the same package but with a different version (v1.2). Therefore, we use venv's to keep the installed packages seperate and allow us to run both scripts simultaneously, without running into any problems.


1. Initilialise VSCode, and open a folder
2. Initilialise a venv
    ```bash
    python -m venv MyVirtualEnvironment
    ```
    You will notice that a new folder is created in the Explorer
3. Activate the venv
    ```bash
    MyVirtualEnvironment/Scripts/Activate.bat
    ```
4. Select the interpreter
    
    We need to select the interpreter that we want our script to be run from. In VSCode go to the "Command Palette" in the "View" tab *(or use the shortcut `Ctrl+Shift+P`)*.

    Search for "Python: Select Interpreter" and some interpreter options will be shown.

    If the intepreter you want is not available, choose "Enter interpreter path" and choose `/MyVirtualEnvironment/Scripts/python.exe`

5. Install packages
    Now you can install whatever packages you want for the venv.
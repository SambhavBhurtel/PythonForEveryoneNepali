# Convert Python script into windows executable!

Hello, now we will be converting our python script into a windows executable file. Please read the paragraphs properly below:


## What are python script?

Until now, you've written all your code in **.ipynb** file but the python interpreter originally executes python scripts which are saved in **.py** format. Then only the **.py** can be converted into **.exe** format.

### Convert the .ipynb into .py:
1. Inside the jupyter notebook, click on **File** menu then on **Download as** and select **python script (.py)**. Your python script should be downloaded now. 
2. Copy the file into your workshop directory and rename it as **calculator.py**

## What is a windows executable?
After you write a python script, you might want to share it with your friends or you might want to run it on other computers having Windows OS. The script will only run if the person has python installed on their computer. So, in order to make your script run on different computers, you have to build your script into an executable of **.exe** format which will open as a program on other compters
*Note: We will be using a library named **PyInstaller** here to compile the code into **.exe** format

```mermaid
graph LR
A[.ipynb file] -- Download as --> B(.py Python script)
B -- used by --> C(PyInstaller)
C -- Compiled into --> D(.exe Windows executable)
```

### Installing PyInstaller
1. Open the folder where you have copied the script into
2. In the address bar of the file explorer, type **cmd** and then press enter. Your console should open up.
3. In the console type **pip install --upgrade PyInstaller** and hit enter. Your PyInstaller should be downloaded and setup automatically now.

## Conversion of .py to .exe
1. In the same console type **pyinstaller  -w -F -n "Calculator" calculator.py** Your building process should start now.
2. After the building process completes, in the file explorer, there should be a **dist** folder inside which your executable will be loacted
3. You can now run the application in any computer with Windows OS

If you are interested in using **PyInstaller** you can follow the official documentation [here](https://pyinstaller.readthedocs.io/en/stable/)

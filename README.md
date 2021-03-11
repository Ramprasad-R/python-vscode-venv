# python-vscode-venv

https://stackoverflow.com/questions/54106071/how-to-setup-virtual-environment-for-python-in-vs-code

With a newer VS Code version it's quite simple.

Open VS Code in your project's folder.

Then open Python Terminal (Ctrl-Shift-P: Python: Create Terminal)

In the terminal:

python -m venv .venv
you'll then see the following dialog: enter image description here

click Yes

Then Python: Select Interpreter (via Ctrl-Shift-P)

and select the option (in my case towards the bottom)

Python 3.7 (venv) ./venv/Scripts/python.exe

If you see

Activate.ps1 is not digitally signed. You cannot run this script on the current system.

you'll need to do the following: https://stackoverflow.com/a/18713789/2705777

For more information see: https://code.visualstudio.com/docs/python/environments#_global-virtual-and-conda-environments

Installing Modules
Ctrl-Shift-P and Terminal: Create New Integrated Terminal

from the terminal

windows: .\.venv\Scripts\activate

linux: .\.venv\bin\activate

you can now instal packages as usual e.g. pip install sklearn

for jupyter, you need to do more Jupyter notebooks in vscode does not use active virtual environment

# .py files
You now know the very basics of Python, hurray! *But how do I write and run Python code outside this course?*

# Let's explain the File Editor and Terminal on Katacoda
**Terminal**<br>
The Terminal is like the Command Prompt on your Windows computer. Using that, you can do everything that you can achieve via mouser and keyboard and more, from creating folders to changing computer settings.

For Week 1 we configured the Terminal to run Python. Katacoda has Python pre-installed within the system and we initialised Python within the Terminal for you by typing either ```python``` or ```py``` depending on the system. Now you can type and run Python code directly from the Terminal!

This will quickly become impractical as your code grows, so let's quit Python by typing this in the Terminal: `exit()`{{execute}}. If you want Python back refresh the page or type this: `python`{{execute}}

**File Editor**<br>
So what's the alternative? The File Editor is a bit like your computer. You can have folders and then files inside of those folders. These files are just like files on your computer - images, videos etc. Pictures might be named ```dog.png``` or ```cutebunnies.jpg``` for example, while we name Python files as ```example.py```. Python files are essentially text files, and we simply name the file extensions as ```.py``` so that programmes know it's a Python file.

In future weeks we'll be creating Python files within the File Editor where we can write much longer code and actually save it. We can then run the Python code via the Terminal.

# Online Python Editors
Want to quickly write and run simple Python code but not install Python on your computer? Try some of these online options!
- [Google Colab](https://colab.research.google.com/)
- [W3Schools](https://www.w3schools.com/python/trypython.asp?filename=demo_compiler)
- [replit](https://replit.com/languages/python3)
- [Visual Studio Code - Browser Version](https://vscode.dev/) (can edit but not run code)

# Python on Computers
If you need help setting this up, don't hesistate to reach out to anyone at VCC, message the Support Channel on Teams, or join our monthly Support Session!

**1. Installing on Windows**<br>
Simply head over to [Python.org](https://www.python.org/) and download Python. <span style="color:red">*The newer 3.x versions of Python may not be widely supported just yet, as of November 2021. Ask a member of VCC for advice or download an older version such as 3.8.5.*</span> Afterwards, open up *Command Prompt* and enter the following to see if Python has been installed: ```python --version```, in which case it will tell you the current version of Python installed, such as ```Python 3.8.5```.

**1. Installing on Windows without Admin Access**<br>
Option A: Go through the same process as above, but when the installer reachers the relevant step uncheck the *install for all users* option.

Option B: Install [Anaconda](https://www.anaconda.com/), which by default should install without requiring admin access.

Option C: Go to the download page for a specific version of Python such as [3.8.5](https://www.python.org/downloads/release/python-385/), download the binary/zip file, unzip the folder, open up *edit environmental variables for your account* through the Windows search bar, edit PATH and add a new entry for where your unzipped folder is. <span style="color:red">*For work laptops, please install approved software via the company IT Shop. VCC does not support any installations that may be against company security rules.*</span>

**1. Installing on MacOS**<br>
Simply head over to [Python.org](https://www.python.org/) and download Python. <span style="color:red">*The newer 3.x versions of Python may not be widely supported just yet, as of November 2021. Ask a member of VCC for advice or download an older version such as 3.8.5.*</span> Afterwards, open up *Terminal* and enter the following to see if Python has been installed: ```python --version```, in which case it will tell you the current version of Python installed, such as ```Python 3.8.5```.

**2. Editing**<br>
You can edit Python code using anything ranging from the pre-installed *Notepad* on Windows or *TextEdit* on MacOS to code editors such as [Visual Studio Code](https://code.visualstudio.com) or [Sublime Text](https://www.sublimetext.com/download). It's ultimately down to personal preference, so ask VCC! <span style="color:red">*For work laptops, please install approved software via the company IT Shop. VCC does not support any installations that may be against company security rules.*</span>

**3. Running on Windows**<br>
Open up *Command Prompt*, [navigate to the folder](https://www.howtogeek.com/659411/how-to-change-directories-in-command-prompt-on-windows-10/) where your Python code is stored, and then type ```python filename.py```.

Alternatively, simply type ```python``` to run Python directly from *Command Prompt*, just like Katacoda's Terminal we have set up to the right.

**3. Running on MacOS**<br>
Open up *Terminal*, [navigate to the folder](https://www.maketecheasier.com/run-python-script-in-mac/) where your Python code is stored, and then type ```python filename.py```.

Alternatively, simply type ```python``` to run Python directly from *Terminal*, just like Katacoda's Terminal we have set up to the right.

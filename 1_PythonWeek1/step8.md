# Python on Computers
If you need help setting this up, don't hesistate to reach out to anyone at VCC, message the Support Channel on Teams, or join our monthly Support Session!
<br><span style="color:red">*The newer 3.x versions of Python may not be widely supported just yet, as of November 2021. Ask a member of VCC for advice or download an older version such as 3.8.5.*</span> 
<span style="color:red">*For work laptops, please install approved software via the company IT Shop. VCC does not support any installations that may be against company security rules.*</span>

<hr>

**1. Installing on Windows**<br>
Simply head over to [Python.org](https://www.python.org/) and download Python. Afterwards, open up *Command Prompt* and enter the following to see if Python has been installed: `python --version`, in which case it will tell you the current version of Python installed, such as `Python 3.8.5`.

**1. Installing on Windows without Admin Access**<br>
Option A: Go through the same process as above, but when the installer reaches the relevant step uncheck the *install for all users* option. This should install without requiring admin access.

Option B: Install [Anaconda](https://www.anaconda.com/), which by default should install without requiring admin access.

Option C: Go to the download page for a specific version of Python such as [3.8.5](https://www.python.org/downloads/release/python-385/), download the binary/zip file, unzip the folder, open up *edit environmental variables for your account* through the Windows search bar, edit PATH and add a new entry for where your unzipped folder is.

**1. Installing on MacOS**<br>
Simply head over to [Python.org](https://www.python.org/) and download Python. Afterwards, open up *Terminal* and enter the following to see if Python has been installed: `python --version`, in which case it will tell you the current version of Python installed, such as `Python 3.8.5`.

<hr>

**2. Editing**<br>
You can edit Python code using anything ranging from the pre-installed *Notepad* on Windows or *TextEdit* on MacOS to code editors such as [Visual Studio Code](https://code.visualstudio.com) or [Sublime Text](https://www.sublimetext.com/download). It's ultimately down to personal preference, so ask VCC!

<hr>

**3. Running on Windows**<br>
Open up *Command Prompt*, [navigate to the folder](https://www.howtogeek.com/659411/how-to-change-directories-in-command-prompt-on-windows-10/) where your Python code is stored, and then type `python filename.py`.

Alternatively, simply type `python` to run Python directly from *Command Prompt*, just like Katacoda's Terminal we have set up to the right.

**3. Running on MacOS**<br>
Open up *Terminal*, [navigate to the folder](https://www.maketecheasier.com/run-python-script-in-mac/) where your Python code is stored, and then type `python filename.py`.

Alternatively, simply type `python` to run Python directly from *Terminal*, just like Katacoda's Terminal we have set up to the right.

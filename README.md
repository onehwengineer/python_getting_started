## python_getting_started
Step-by-step tutorial on getting started with Python in MacOS Big Sur

- [0] Check if **Python3** is already installed
  - In Terminal, `python3 —version`
  - If Python3 is installed, it will show the version. If not, an error.

- [1] Install **Xcode** (along with **Command Line Tools** and **Git**)
  - Check if Xcode is already installed. In Terminal, `- xcode-select -p`
    - If directory exists, Xcode is installed   
    - If not, install Xcode from App Store
  - Check if Git installed : `git --version`
  - **Xcode Command Line Tools** will be installed in step [2]

- [2] Install **Homebrew** (& **Command Line Tools**)
  - Homebrew is a package manager that let's you install stuff that Apple or Linux didn't need
  - Homebrew is made with Ruby, so it will be modifying your computer’s Ruby path. 
  - Open Terminal, and paste :
  - ```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"```
    - The curl command pulls a script from the specified URL. 
    - This script will explain what it will do and then pauses the process to prompt you to confirm. This provides you with a lot of feedback on what the script is going to be doing to your system and gives you the opportunity to verify the process.  
  - Confirm Homebrew installation, `brew doctor`
  - This will also install **Xcode Command Line Tools** (this step takes a while... 2.5GB)
    - Confirm installation by `xcode-select -p` -> Directory will show up (.../CommandLineTools)

- [3] Install **Python3**
  - ```brew install python```
  - Along with Python 3, Homebrew will install pip3, setuptools and wheel
  - TO UPGRADE : `brew upgrade` + `brew upgrade python3`

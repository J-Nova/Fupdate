# Fupdate (Full update)
All in one command to update all brew packages/cask's and pip packages that are installed on your system to their latest versions.
Tested and working on Macbook M1 w MacOS Monterey version 12.2

__________________

Requirements:
Install https://github.com/buo/homebrew-cask-upgrade in your terminal via brew with the command `brew tap buo/cask-upgrade`

__________________

Step 1:
Open your terminal and open up `.zshrc` (or equivalent for your OS) via the terminal editor `nano`.
You can do this with the command `nano .zshrc`.

Step 2:
Once the file editor has opened up copy-paste this `alias fupdate="brew update; brew upgrade; brew cu --all; brew cleanup; pip3 install -r <(pip3 freeze) --upgrade"` on a new line at the bottom of the file. Next Exit the file editor with the key combination of (on MacOS) `control + X`. And press Y to save the edited file.

Step 3:
Exit your opened terminal and open a new fresh terminal to be able to use the added command `fupdate`.

__________________

With the command / alias you have added you are now able to update & upgrade all installed brew & pip packages on your system with only one command. 

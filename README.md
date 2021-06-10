# git-crypt compiled for Windows 64 bit
This repository contains an .exe of git-crypt 0.6.0 that runs on Windows 64 bit machines. It has been tested to work in Windows 10. Note that as of 10.06.2021 git-crypt for Windows is still experimental according to the [git-crypt repo](https://github.com/AGWA/git-crypt/blob/master/INSTALL.md#experimental-windows-support) with the following caveat: "Windows support is less tested and does not currently create key files with restrictive permissions, making it unsuitable for use on a multi-user system."

## Setup
Download the .exe file and put it anywhere. Then add the path to the folder containing the .exe to your Path environment variable. For example, for me I added a new row to the Path variable for my user's environment variables that is C:\Code\Askeladden\programmer\git-crypt-windows.

No further installation is necessary.

## How this was created
I followed [this stackoverflow guide](https://stackoverflow.com/questions/43040370/how-to-install-git-crypt-on-windows) including the steps specified in the comments. Except that running 'make' in the m2sys terminal did not work for me, but doing it in the mingw64 terminal did (mingw64.exe after you install m2sys). I also made sure to do the step in the stackoverflow post's comments specifying to compile the mentioned libaries into the .exe so that it can be ran anywhere.

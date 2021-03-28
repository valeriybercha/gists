# Apps to install on Debian Linux operating system

1. VLC media player – ```sudo apt install vlc```
2. GIMP – ```sudo apt-get install gimp```
3. VIM – ```sudo apt install vim```
4. Git – ```sudo apt install git```
5. Notepad++
* ```sudo apt install snapd``` (install snap first)
* ```sudo snap install notepad-plus-plus``` (install notepad++ via snapd)
* ```snap run notepad-plus-plus``` (run the app)
6. Ulauncher (ulaunher.io) 
* download .deb package
* ```sudo apt install ./package.deb```
7. Stacer 
* ```sudo add-apt-repository ppa:oguzhaninan/stacer```
* ```sudo apt-get update```
* ```sudo apt-get install stacer```
8. Timeshift (system backup) - ```sudo apt install timeshift```
9. Neofetch – ```sudo apt install neofetch```
10. Pycharm community edition - ```sudo snap install pycharm-community --classic```
11. Virtualenv install:
* ```sudo ap-get install python3-pip``` (install pip)
* ```sudo pip3 install virtualenv``` (install virtualenv from pip)
12.  Install and configure VS Code for Ubuntu:
* ```sudo snap install --classic code``` (VS Code is distributed as a snap package) or install vs code as a .deb package – download the package from - [https://code.visualstudio.com/docs/setup/linux](https://code.visualstudio.com/docs/setup/linux) and run ```sudo apt install ./<file>.deb``` command
* ```sudo apt install python-is-python3``` (running python 3 version in VS code)
13.  Install Sublime Text editor:
* ```wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add``` (install the GPG key)
* ```sudo apt-get install apt-transport-https```
* ```echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list``` (stable channel for installing)
* ```sudo apt-get update``` (update apt sources)
* ```sudo apt-get install sublime-text``` (install sublime text on ubuntu)
14.  Google Chrome install from terminal:
* ```wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add``` – (download repository key)
* ```sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list``` (add a repository)
* ```sudo apt-get update``` (update)
* ```sudo apt-get install google-chrome-stable``` (install chrome stable version)
15. Install Indicator Multiload (CPU and RAM usage icon in the top bar) - freezed for me the Gnome so I had to uninstall it:
- ```sudo apt install indicator-multiload```
- ```sudo apt-get purge --auto-remove indicator-multiload``` (remove the app and it's dependencies)
16. Install htop
- ```sudo snap install htop``` (install over snap)
- ```sudo apt install htop``` (install via apt)
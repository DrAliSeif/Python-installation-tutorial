# Python-installation-tutorial
## Setup python on Linux in Windows using WSL and VS Code
Training on installing and using Python in the VS code environment for Windows and running Python in Ubuntu using wsl and displaying plots using xming and connecting codes in Github to use Git

### you can use an X server to enable graphical support in WSL.
1. Install an X server on your Windows 10 machine. One popular option is Xming, which you can download from the official website: https://sourceforge.net/projects/xming/
2. After installing Xming, launch it from the Start Menu or desktop shortcut. Make sure the Xming server is running.
3. In the WSL Ubuntu terminal, set the DISPLAY environment variable to point to your Windows machine's IP address. You can find the IP address by running the following command in a Command Prompt window on your Windows machine:
ipconfig
Look for the "IPv4 Address" under the network adapter you're using (e.g., Ethernet or Wi-Fi). It should be a series of numbers separated by dots (e.g., 192.168.1.100).
In the WSL terminal, run the following command, replacing `<Windows IP>` with the IP address you found:
export DISPLAY=<Windows IP>:0.0'''
(For example, if your Windows IP address is 192.168.1.100, the command would be: export DISPLAY=192.168.1.100:0.0)
4. Now, when you run your Python code with plt.show(), the plot should be displayed on your Windows desktop. Ensure that you have the necessary Python packages (e.g., matplotlib) installed in your WSL Ubuntu environment.

### use wsl in vs code
1. open vs code
2. go to the extensions
3. install WSL
4. oppen remote host
5. connect to wsl or reopen folder in wsl
6. go to the extensions
7. install python(Extension is enabled on 'WSL: Ubuntu')
8. run program
9. open select python interpreter

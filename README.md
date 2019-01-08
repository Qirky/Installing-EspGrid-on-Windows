# In-depth instructions for installing EspGrid on Windows machines

[EspGrid](https://github.com/d0kt0r0/EspGrid) is a powerful tool for synchronising live coding environments over a network and was developed by David Ogborn. Configuration can be a bit tricky on Windows as it requires a few downloads so this is a quick run through of how to get installed and what might go wrong / how to fix it.

# Steps

- Go to gnustep.org/windows/installer.html
- Scroll to "Download" and download the GNUStep MSYS System and GNUStep Core libraries by clicking their respective stable release numbers
- Once downloaded, install each library by double clicking on them
- Restart your computer
- Try running EspGrid.exe
- If you get errors, add C:/GNUStep/bin to your system path (or wherever you installed the libraries) and try again - see below for more help on this
- If you still get errors, move the espgrid.exe file to the C:/GNUStep/bin folder and try again.

# Adding a directory to your system path

- Go to file explorer, right click on My Computer / This PC or similar and press "Properties"
- Go to "Advanced system settings" and click on the "Environment Variables" button near the  bottom
- There should be a variable called PATH and its value should have some directory names. Click on Edit... If it is not there, create a new variable called PATH.
- On Windows 8 and earlier, add C:/GNUStep/bin to the variable value field but make sure you add a ; to the end of the last folder name.
- On Windows 10, click New and enter C:/GNUStep/bin
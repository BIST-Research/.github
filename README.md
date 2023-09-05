This GitHub organization houses code and other materials related to the active development pertaining to research conducted through the Bio Inspired Sciences and Engineering lab (BIST) at Virginia Tech. 

#Embedded code

## VSCode, PlatformIO and uploading code

First, install [VSCode](https://code.visualstudio.com/Download) and the [PlatformIO](https://platformio.org/install/ide?install=vscode) extension. 

Create a new project in PlatformIO. If the PIO screen does not show when opening VSCode, check the left side of the toolbar at the bottom of the window for a house icon and click it. It may take a few seconds after opening VSCode for PIO to launch so give it a few seconds for the house to show. 

Select the board being used. The MCU sent inside bb6 is the ```Adafruit Itsybitsy M4```. Note that the board selection dropdown can also be typed in to filter results.

The name you choose for the project doesn't matter.

Once the project is created, you should see a file navigation window on the left side of the window. If you view inside the ```src``` directory, there should be an autogenerated "main.cpp" file. You can delete this. The source code includes the main structure, so keeping this one will cause namespace issues. 

Now, navigate to the git folder and copy the contents of ```echo_src/src/``` to the PlatformIO project folder. For linux and MacOS users, PIO's default project locations are at ```~/Documents/PlatformIO/```.

Now, go back to VSCode, and the ```src``` directory should be holding the project source code. Look for a check mark icon in the bottom toolbar to compile the code for errors. 

Next, connect the microcontroller and verify that PIO sees it by pressing the PIO home button (bottom tool bar) and going to the "devices" section in the left hand toolbar. If it doesn't show, see the "Updating the MCU bootloader" section of this readme.

Press the arrow icon in the bottom toolbar to upload the code. If the upload process hangs on ```waiting for new upload port``` and then fails, double tap the reset button on the MCU and try reuploading. 

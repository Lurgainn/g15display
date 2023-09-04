# g15display
Daemon to manage **Logitech g15/g510's** display for uinput-macropad.  
This program is a part of a suite that under Linux OS controls the functionality and appearance of the keyboard Logitech G510 (and perhaps G15, but this is not tested).  
## Prerequisites
To achieve the full functionality of this program:
* Linux kernel version must be >= 5.5
* The package "g15daemon" must be **NOT** installed
* The package "libg15render" must be installed
* You have to install "lcdproc" from [Github repository](https://github.com/lcdproc/lcdproc); in this way you are sure to have a package within the g15 driver that use hidraw interface
* You must have installed "uinput-macropad.py" that uses the default path of config file (~/.config/uinput-macropad/config.json) or give the option -c </full/path/to/config/file/filname.json>
## Functionality
The program read the uinput-macropad.py config file and configures the keyboard LCD to display the names of the actual existent macros  
> [!NOTE]  
> uinput-macropad must manage the switch between the display screens
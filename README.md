# flutter_desktop_linux_graphic_bug_fixed
Fix Nvidia bug on Flutter desktop app runner

We will Talk About bug fixing
on "[FATAL:flutter/shell/gpu/gpu_surface_gl_delegate.cc(53)] Check failed: gl_version_string. The GL proc resolver's glGetString(GL_VERSION) failed Error waiting for a debug connection: The log reader stopped unexpectedly, or never started. Error launching application on Linux." error

## Step to reproduce

# From The Gui
- Go on Driver setting by searching in the search bar
![Example screenshot](./1fix.png)

- Open Application and select the driver version which is open source then click on apply changes
![Example screenshot](./2fix.png)


- Go in your fluuter project and open it in your editor
- run "flutter clean" command
- run "flutter create --platforms=linux ." command
- run "flutter run -d linux" command your app is working now


# Frome de Command-line interface 

If you prefer the command-line interface, you can use the ubuntu-drivers tool.
Open your terminal (Ctrl+Alt+T), and run the following command to get information about your graphic card and available drivers:
# "ubuntu-drivers devices"

![Example screenshot](./3fix.png)


Then from the results installs the driver with the "distro free builtin" Tag wth command :
# "sudo apt install xserver-xorg-video-nouveau"

![Example screenshot](./4fix.png)



# Thanks
Created by [@fermatdev](https://www.mailto:aimericpouga28@gmail.com) - feel free to contact me!

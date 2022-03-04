# flutter_desktop_linux_graphic_bug_fixed
Fix Nvidia bug on Flutter desktop app runner

We will Talk About bug fixin on "[FATAL:flutter/shell/gpu/gpu_surface_gl_delegate.cc(53)] Check failed: gl_version_string. The GL proc resolver's glGetString(GL_VERSION) failed Error waiting for a debug connection: The log reader stopped unexpectedly, or never started. Error launching application on Linux." error

## Step to reproduce
- Go on Driver setting by searching in the search bar
![Example screenshot](./1fix.png)
- Open Application and select the driver version which is open source then click on apply changes
![Example screenshot](./2fix.png)
- Go in your fluuter project and open it in your editor
- run flutter clean
- run flutter create --platforms=linux .
- run flutter run -d linux your app is working now


# Thanks
Created by [@fermatdev](https://www.mailto:aimericpouga28@gmail.com) - feel free to contact me!

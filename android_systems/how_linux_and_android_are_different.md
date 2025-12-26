# How Android and Linux Systems are different
We know that **Android** uses **[Linux Kernel](https://en.wikipedia.org/wiki/Linux_kernel)** but still both of them are much different when we tries using the command line interface.

## Basic Changes I found
1. Filesystems in android are different from GNU Operating Systems (Ubuntu, Debian, etc)
2. Linux uses **glibc**, **GNU Core Utilities**, ***/etc, /home, /var, /log Layout**, **X11/Wayland display Servers**
3. Android uses **Bionic Libc**, **Its Own Toolchain**, **/system, /vendor, /data Layout**, **No X11/Wayland**, **Java/Kotlin-first runtime(ART)**

Basically, A linux applicatino asks for things that simply don't exist on Android.

# References
Android -> [Android_Operating_System](https://en.wikipedia.org/wiki/Android_(operating_system))
Linux -> [Linux Operating System](https://en.wikipedia.org/wiki/Linux)

# Materials
- You can download **Android** from **[Here](https://www.android-x86.org/)**.
- You can download **Linux** from **[Here](https://www.linux.org/pages/download/)**, I choose this website because it shows alomst every linux distribution.

You guys can download the respective operating systems and try running them setup on a **Virtual Machine** and try to find out how they works.
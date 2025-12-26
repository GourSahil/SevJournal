# KUL-739B :: How Android and Linux Systems Are Different


We know that **Android** uses the **Linux kernel**, yet both systems behave very differently—especially when interacting through the command-line interface.

This difference exists because Android and traditional GNU/Linux systems are built with **entirely different userland designs**, even though they share the same kernel.

---

## Basic Differences Observed

1. **Filesystem layout** in Android is different from that of GNU/Linux operating systems (such as Ubuntu, Debian, etc.).

2. Traditional Linux systems rely on:
   - **glibc**
   - **GNU Core Utilities**
   - Standard filesystem layout (`/etc`, `/home`, `/var`, `/log`)
   - **X11 or Wayland** display servers

3. Android, on the other hand, uses:
   - **Bionic libc**
   - Its own toolchain
   - Android-specific layout (`/system`, `/vendor`, `/data`)
   - No **X11/Wayland** display server
   - A **Java/Kotlin-first runtime (ART)**

---

## Key Insight

> A Linux application expects components that **simply do not exist** in Android’s environment.

This is why Linux desktop applications cannot directly run on Android systems without compatibility layers or containerized environments.

---

## References

- Android: https://en.wikipedia.org/wiki/Android_(operating_system)  
- Linux: https://en.wikipedia.org/wiki/Linux  

---

## Materials for Practice

- Download **Android (x86)** from:  
  https://www.android-x86.org/

- Download **Linux distributions** from:  
  https://www.linux.org/pages/download/  
  *(This site conveniently lists most available Linux distributions.)*

---

You can install both operating systems inside a **virtual machine** and explore their filesystems, process models, and command-line behavior to better understand how they differ in practice.

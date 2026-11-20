Astra-OS
=========

A fully functional, feature-rich operating system from scratch. Everything is written from the ground up: a custom UEFI bootloader, a 64-bit SMP kernel, a compositing desktop, and everything in between.

## Design Goals

- **Windows 11 where it matters.** Win32 is the native API, paths look like C:\Impossible\System32\, and the desktop follows Windows 11 closely, with a slightly frostier glass.

- **Linux where it widens reach.** Linux binaries are planned through a compatibility layer, not a renamed POSIX API.

- **Bare metal first.** Virtual machines are for fast iteration. A feature is done when it works on real hardware.

- **SMP from day one.** Per-CPU data, real locking and atomics everywhere, with no big kernel lock to remove later.
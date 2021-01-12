# general
There are so many emulators out there and such great code that's it's hard to keep track. I will attempt to do it here. My main interest is emulators and supporting software that runs on Linux in general and Raspberry Pi's (currently Pi4 and Pi400) in particular. Pulls and forks will likely be an effort to adjust / improve compatibility for Pi.

# Apple I Emulators

# Apple III Emulators

# Apple II Emulators
Wow! So many it's hard to list them all. Here are some that stand out
AppleWin. Although this project is built for Windows, there's a Linux port under way that intends to continue to incorporate updates from the parent project in a sustainable manner. AppleWin is really the "gold standard" for Apple II emulation, both in terms of fidelity and supported features.
LinApple(II). This fork of LinApple (itself originally forked from AppleWin) has historically been the most advanced option for Apple II emulation on Linux and is what is included with the RetroPie distribution.
Apple2. According to the author, this emulator derived from ApplePC. Quite useful as ApplePC has faded into the sands of time. This emulator isn't as feature rich as LinApple or AppleWin, but is interesting since it's a unique perspective.
Apple2 (https://github.com/mauiaaron/apple2) is based on Apple2ix and is interesting as it includes ARM assembly emualation for the 65c02 CPU.

# Apple IIgs Emulators
KEGS. Kent Dickey's venerable IIgs emulator. Development seems to have stopped in the mid-noughts, but GSPort and GSPlus carry on its code legacy.
XGS. Joshua Thompson began work on this IIgs emulator around the same time that work began on KEGS. A few derivative versions seem to have floated around for IIgs emulators on M68K machines, but there doesn't seem to be any modern derivatives (other than a project that builds on the 68816 CPU emulation code). Unlike KEGS, however, development on XGS never stopped and the developer is focused on bringing the emulator to the Pi. This is also the only C++ based IIGS emulator.
GSPort and GSPlus. These are both derived from KEGS, are Linux compatible, and share quite a bit of the same functionality. GSPlus seems to largely be the successor to GSPort.
Gus. This was a project unofficially supported by Apple, apparently with some work done at University, to bring IIgs support to PPC machines. It's unclear whether the code was ever released in compiled form for M68K machines, but it appears the code is set up to allow cross-compilation. It's possible that the M68K machines at the time didn't have the computing power to run Gus at an acceptable speed, but that's likely a non-issue today. Although it appears that other IIgs emulators drew inspiration from Gus (and are now more feature rich), Gus is interesting in that it contains an M68K and PPC assembly version of the CPU emulation component as well as some memory tricks for additional speed.

# M68K Mac Emulators
OS 9. With its built-in Rosetta translator, it may actually provide the broadest range of Classic software compatibility, but does require a PPC emulator as support for M68K processors was dropped at OS 8.1
Basilisk II was the predecessor to SheepShaver and shares a fair amount of code. Available on multiple platforms with varying degrees of stability. Performant, even on Pi.
Mini vMac is another classic M68K processor. Originally built to emulate the earliest 68000 machines, it is now capable of emulating a broad range of M68K CPUs and OS versions. Lots of forks for this emulator, I'll try to track the most up-to-date.
Advanced Mac Substitute
This is similar to Executor, in that it aims to be able to run Classic software without a proprietary ROM image, but seems to be a lot more mature. Seems to be best suited to running old OS 6 software, but would make a great "clean room" implementation if sufficient attention were focused on it.

# PPC Mac Emulators
QEMU is able to emulate a PPC Mac with certain limitations. Depending on how it is compiled, it can run at an acceptable speed for Pre-OS X environments.
SheepShaver is able to emulator a PPC Mac (also with certain limitations). It is generally more performant than QEMU, but maybe not as stable.
Others?

# Emulator Support Tools
Although they don't qualify as emulators, the following software is key to getting maximum usage of the above emulators.

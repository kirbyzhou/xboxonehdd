Xbox One HDD Tools
==================

What this does
--------------

Given any HDD over 500GB in size, you can format it for use with your Microsoft Xbox One console


How
---

![Magic](http://i.imgur.com/56WNIjG.gif)


Instructions
------------

All of this must be done as root!
You can run it under linux/macOS with NTFS support.
Or you can run it with linux/macOS + Windows.
I HIGHLY suggest you do this on a livecd or usb booted system if you don't 'know linux' and would rather not wipe the wrong hard drive.
For macOS, you can install ntfs-3g by brew(https://brew.sh).

1. Connect your HDD and take note of what its called (ex: sda, sdb under linux, disk3, disk4 under macOS etc )
2. Run the script with the device name as the first parameter
3. It will bitch about missing partitions etc, but write a file with commands to create said missing partitions
4. Run the created script
5. [Optional] Go windows to format the newly created partitions as NTFS
6. Copy the correct files to the newly created partitions
7. [Optional] Go back to linux/macOS
8. Unmount the newly created partitions
9. Run the main script again


Putting it back together
------------------------

When you put the new HDD in your console for the first time and boot up, the console will go the the green "Xbox One" screen, pause for a second or two, then shut down. Boot the console again.  This time it should pause at the green screen for a while longer, then go to a black screen for even longer.  It can take several minutes before anything happens after this, the xbox is automatically creating temporary files during this time.  If you copied everything correctly, it WILL go to the dashboard eventually, just be patient!


What is linux?
--------------

Wait for a windows version


Required Files
--------------

These can be gotten off your original HDD easily

```
└── [4.0K]  System Update
    ├── [4.0K]  A
    │   ├── [341M]  deltas.xvd
    │   ├── [ 36M]  SettingsTemplate.xvd
    │   ├── [ 24M]  sosinit.xvd
    │   ├── [ 62M]  sostmpl.xvd
    │   ├── [267M]  systemaux.xvd
    │   └── [850M]  system.xvd
    ├── [4.0K]  B
    │   ├── [ 30M]  SettingsTemplate.xvd
    │   ├── [ 23M]  sosinit.xvd
    │   ├── [ 45M]  sostmpl.xvd
    │   ├── [ 91M]  systemaux.xvd
    │   └── [761M]  system.xvd
    └── [ 44M]  updater.xvd

```

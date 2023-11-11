The better way to apply changes:
1. Use git bash on computer 
2. From git get into the main directory (where this file is actually)
3. Enter 'code .' to open the whole repository in Visual Code
4. After complete editing all files use git to push it to Github:
4.1. Add all changes to git log by 'git add .'
4.2. Commit changes with a message 'git commit -m "some message"'
4.3. Push changes to GitHub by 'git push'
5. In the GitHub (on web) in the respective repository open Actions tab to see progress of the build workflow
6. Once the build successfully completed, find inside the firmware.zip file
7. Inside the zip file there are 2 UF2 files for each half of the keyboard (in case of split keyboard)
8. To get into bootloader mode on the nRf52 (Nice!nano, XLE BLE) boards - connect to computer via USB and double-press on the reset button
9. In the bootloader mode the MicroComputingUnit board will appear in Windows as a files drive
10. Copy the UF2 file of the respective keyboard side to that drive. The board will reboot itself
11. We are done!

Enjoy!
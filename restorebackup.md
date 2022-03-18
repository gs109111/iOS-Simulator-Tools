

# Restore Simulator To "Real" iPhone Backup v1.0
<a href="https://gs109111.github.io/iOS-Simulator-Tools/">Home</a>

1. Create a Backup of the iPhone using finder or itunes
2. Download iBackupBot to extract the backup 
3. Open iBackupBot
4. Select the directory of the backup
5. In the Application, go the System Files > Home Domain > Library
6. Copy / Extract All The Folders and Files in this directory to anywhere on your mac
7. Head over to /Library/Developer/CoreSimulator/Devices 
8. Use the DeviceSet.plist file to find out what device UDID matches up with what device you need
9. Open the Correct folder for the device
10. Open Data > Library
11. Backup all the content of the Library folder to a diffrent directory on your mac (For future removal)
12. After backing up all the content remove all the content in this directory
13. Copy the contents of the backup you extracted earlier to this directory (Library)
14. Start up the simulator
15. Your iCloud Account will be logged in, the wallpaper will be the one from the device and some other features will be the same. 
16. Note: You are not able to install the apps on your iDevice to the simulator

# Remove Backup
1. Simply delete the content in the /Library/Developer/CoreSimulator/Devices/UDID/Data/Library/
2. Copy the content you backed up on your mac to this directory (In Step 10)

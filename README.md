# iOS-Simulator-Dualboot Writeup v1


No Patches Required !!!

100% All Downloads are from Apple 
iOS 10.3.1: https://devimages-cdn.apple.com/downloads/xcode/simulators/com.apple.pkg.iPhoneSimulatorSDK10_3-10.3.1.1495751597.dmg
iOS 9.3.1: https://devimages.apple.com.edgekey.net/downloads/xcode/simulators/com.apple.pkg.iPhoneSimulatorSDK9_3-9.3.1.1460411551.dmg
The Downloads are just extracted for you

Dualboot iOS 12.4 & iOS 9.3 - 12x on iOS Simulators (Older iOS Versions May Work?)

Support: Xcode (Including Xcode 13)

Tested On:
Xcode 13.2.1 
iOS 12.4 (As Main OS)
iOS 10.3.1 & iOS 9.3 (Secondary OS)
iPhone 5s, 6, 6s, 6plus

I have not tested other iOS Versions other than iOS 9.3 and iOS 10.3.1 and other simulator runtimes (e.g iOS 15 runtime).


# Boot iOS 10.3.1 

1. Download the iOS 12.4 Simulator runtime in Xcode (Xcode > Prefrences > Components)
1. Download The RuntimeRoot + SampleContent.zip-iOS10 File From https://mega.nz/file/T3wQhQ6A#s_Rm5BiP1W8gN11gVBa4YsMCR-fwO7AXty_01GBU1gU and extract it anywhere.
2. Open Finder and Go to the /Library/Developer/CoreSimulator/Profiles/Runtimes directory
3. Right Click the iOS 12.4.simruntime and select show package contents
4. Click on the Contents folder and then click on resources
5. IMPORTANT: Backup the iOS 12.4 Simulator by renaming the RuntimeRoot in the resources folder to RuntimeRoot-iOS12 and Sample Content in the resources folder to Sample Content-iOS12
6. Copy the Runtime Root and SampleContent you downloaded from the link to the current directory (/Library/Developer/CoreSimulator/Profiles/Runtimes/iOS 12.4.simruntime/Contents/resources)
7. Open the iOS Simulator app and select iOS 12.4 and Any Supported Device (E.g. iPhone 6) in file > open simulator menu
8. It may take sometime to boot the simulator and the wallpaper will be the current iOS 12.4 wallpaper but the os will be iOS 10.3.1

# Boot iOS 9.3.1
1. Download the iOS 12.4 Simulator runtime in Xcode (Xcode > Prefrences > Components)
1. Download The RuntimeRoot & Sample Content Folder From https://mega.nz/file/P3AHlQLS#_9DiohpwLLdu2-Gjv-2V9cZIgv6_u8tzfTcLO45papQ and extract it anywhere.
2. Open Finder and Go to the /Library/Developer/CoreSimulator/Profiles/Runtimes directory
3. Right Click the iOS 12.4.simruntime and select show package contents
4. Click on the Contents folder and then click on resources
5. IMPORTANT: Backup the iOS 12.4 Simulator by renaming the RuntimeRoot in the resources folder to RuntimeRoot-iOS12 and Sample Content in the resources folder to Sample Content-iOS12
6. Copy the Runtime Root and SampleContent you downloaded from the link to the current directory (/Library/Developer/CoreSimulator/Profiles/Runtimes/iOS 12.4.simruntime/Contents/resources)
7. Open the iOS Simulator app and select iOS 12.4 and Any Supported Device (E.g. iPhone 6) in file > open simulator menu
8. It may take sometime to boot the simulator and the wallpaper will be the current iOS 12.4 wallpaper but the os will be iOS 9.3.1


# Go Back To iOS 12.4 Or Remove The Dualboot


Go Back (Dualboot):
1. Rename the RuntimeRoot to RuntimeRoot-iOS10 or RuntimeRoot-iOS9 and SampleContent to SampleContent-iOS10 or SampleContent-iOS9
2. Rename the RuntimeRoot-iOS12 to RuntimeRoot and SampleContent-iOS12 to SampleContent

Remove iOS 10.3.1:
1. Delete the SampleContent-iOS10 and RuntimeRoot-iOS10

Remove iOS 9.3.1:
1. Delete the SampleContent-iOS9 and RuntimeRoot-iOS9

Some Features Of The iOS Simulator Might Be Broken (During iOS 10.3.1 or iOS 9.3.1) , But the OS should work fine


========================================================================


# Restore Simulator To "Real" iPhone Backup v1
1. Create a Backup of the iPhone using finder or itunes
2. Download iBackupBot to extract the backup 
3. Select the directory of the backup
4. In the Application, go the System Files > Home Domain > Library
5. Copy / Extract All The Folders and Files in this directory to anywhere on your mac
6. Head over to /Library/Developer/CoreSimulator/Devices 
7. Use the DeviceSet.plist file to find out what device UDID matches up with what device you need
8. Open the Correct folder for the device
9. Open Data > Library
10. Backup all the content of the Library folder to a diffrent directory on your mac (For future removal)
11. After backing up all the content remove all the content in this directory
12. Copy the contents of the backup you extracted earlier to this directory (Library)
13. Start up the simulator
14. Your iCloud Account will be logged in, the wallpaper will be the one from the device and some other features will be the same. 
15. Note: You are not able to install the apps on your iDevice to the simulator

# Remove Backup
1. Simply delete the content in the /Library/Developer/CoreSimulator/Devices/UDID/Data/Library/
2. Copy the content you backed up on your mac to this directory (In Step 10)


All Copyright Goes To Apple

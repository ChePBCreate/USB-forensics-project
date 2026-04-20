# USB DRIVE FORENSICS & FILE RECOVERY PROJECT

DISCLAIMER:
This project was conducted in a controlled environment using self-created disk images. No real devices or third-party data were used or harmed in this project.

## Overview:
This project demonstrates a basic digital forensics investigation using a virtual USB drive.
I created a disk image, added images and one text file to it, and analyzed the files using Autopsy to recover two deleted files.

## Tools used:

Kali Linux - Forensic operating system
VirtualBox - Virtual environment
Gnome Disks - Virtual disk image creation
Autopsy - Disk image analysis and file recovery
Thunar - File management on host system

## Environment:
Host Operating System - Linux XFCE
Guest Operating System - Kali Linux on VirtualBox VM
Image type - Raw disk image (.dd)
Filesystem - FAT32 
Image size - 1 GB

## Project Steps:
1. Created 1GB virtual disk image using Gnome Disks
2. Formatted image as DOS/MBR
3. Added test photos and text document to the image via Thunar
4. Deleted one photo and text document to late data loss
5. Shared image with Kali Linux VM via VirtualBox shared folder
6. Copied image to Kali and verified file integrity
7. Opened image in Autopsy for forensic analysis
8. Located and recovered deleted files from '.Trash-1000'

## Key findings:
Total files on image: 5
Deleted files recovered: 2
Recovered files: john-doe-id.webp and Passwords text file
Filesystem: FAT32
Partition type: DOS/MBR
Recovery success: 100%

## Screenshots
All screenshots are located in the '/screenshots' folder.

-screenshot1.jpg: shared folder creation on host system
-screenshot2.jpg: Gnome Disks image creation
-screenshot3.jpg: Image formatting
-screenshot4.jpg: Partition creation
-screenshot5.jpg: Image mount on host machine
-screenshot6.jpg: Adding files onto image disk
-screenshot7.jpg: Deleted files off image disk (john-doe-id.webp, Passwords text file)
-screenshot8.jpg: Loaded shared file onto Kali
-screenshot9.jpg: Set up Shared folder and verfied image mount
-screenshot10.jpg: Copied image and verified copied image
-screenshot11.jpg: Loaded Autopsy
-screenshot12.jpg: Created new case
-screenshot13.jpg: Added new image to case
-screenshot14.jpg: Added basic host details
-screenshot15.jpg: Selected file system details
-screenshot16.jpg: Loaded image onto Autopsy for analysis
-screenshot17.jpg: Image file contents showing deleted files
-screenshot18.jpg: Contents of /.Trash-1000 folder
-screenshot19.jpg: Extraction of john-doe-id.webp image via Extract function
-screenshot20.jpg: Extraction of Passwords text file via Extract function
-screenshot21.jpg: Recovered files shown in Downloads folder

## Skills Demonstrated:
- Beginner digital forensics methodology
- Disk imaging and mounting
- File recovery from unallocated space
- Use of open-source forensic tools
- Documentation and reporting
- Virtual machine configuration



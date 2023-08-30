# K1 firmware files
Better organized firmware for the Creality K1 printer

**######## FOR EXPLOITED/ROOTED MACHINES ONLY ########**

This is a different and more clear organization of the config files.
Everything has been separated by theme, like bed leveling, macros, etc.
It should give an easier time looking for any parameter.
If you need to change anything, please do not edit the included files.
Use the "USER OVERRIDES" section bellow, paste what you need and it will 
override the values on the included file.
I'm working on using the biggeste are possible and on changing the fans names.
As soon as I take care of it, I will update the repo.

As some of you may know, on every restart/boot of the machine, it copies the stock files from a folder, 
removing every major changes you have made.
In order to make the changes permanent, you need to edit a file almost like we have to do with moonraker.
(If you want/need to make the moonraker changes, check [this link](https://github.com/Guilouz/Creality-K1-and-K1-Max/wiki/Permanent-Moonraker-Configuration), thanks to Guilouz.


**Make permanent Klipper configuration**
- Connect to SSH (Guide is available here) and go to the folder /etc/init.d/ on the left side of the window:
![1](https://github.com/3dprintpt/K1_organized_firmware/assets/86446936/36361321-6a7e-46d3-b25d-02850749af0b)

- Locate the S55klipper_service file and right click on it and select Open with default text editor:
![2](https://github.com/3dprintpt/K1_organized_firmware/assets/86446936/6fd9c826-0abe-48fb-afe4-a8c5e1e5a68f)

- Comment or delete the complete "copy_config()" section (like in the image).
  ![3](https://github.com/3dprintpt/K1_organized_firmware/assets/86446936/778d7b49-6a13-4884-9d65-62523d8f1731)

- Click the save button and then click on "yes" when you are prompted to upload the changes to the machine.
![4](https://github.com/3dprintpt/K1_organized_firmware/assets/86446936/5ad0b94a-ab8c-4327-ad45-71cf27c78fcd)
![5](https://github.com/3dprintpt/K1_organized_firmware/assets/86446936/903d2217-52e0-46b7-8f6d-d8fc601eb199)

Now you can make any changes you need.
Either my files shared on this repo or any other firmware files.
If you use my files, keep the structure as is. K1 folder with all the includes inside.
You can delete everything from your printer but not moonraker.conf and timepalse.cfg (if you have it).

Enjoy, hope this is useful.

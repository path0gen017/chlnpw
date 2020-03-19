# chlnpw
A software utility that enables one to view active accounts and change their passwords in linux-based operating systems by modification of the shadow file.

This software is free of charge and licensed under the GNU General Public License and inspired by chntpw which is a an offline NT password editor.
It is written in bash and python(works on both version 2 and 3)
Due to the above reason,this utility only works on linux-based operating systems such as kali-linux,parrot OS,ubuntu and the like. 

What does this program do?
__________________________

Primarily,this small program enables one to:
1.view all existing user accounts in the system
2.view the corresponding hashes,the salt used and the algorithm utilized to come up with the hash.
3.change any user's password.

Note:You don't need to know the user's old password in order to change it.This is the main reason as to why I wrote this program

However,note that you need root privileges in order to make this change.This,however,can be bypassed by booting the operating system on a live boot media and making the change on the host's operating system from this media.

How does it work?
_________________
Well,the shadow file located in the ///etc directory is the de facto storage location for usernames and passwords on most linux systems.
This program opens up this file,picks out the usernames and corresponding hashes amidst a host of many other useless stuff(in the context of this program),and then displays them on the screen.If you please,you can still use this software to edit the same file,effectively changing the users' passwords.

If you want specific details of how it does this,then check out the source files.

How do I use it?
________________
Clone or download this repository on a linux system.cd into the chlnpw-* directory and run the chlnpw script which a bash program the main starting point for this utility.Also,please ensure that the other .py scripts are in the same directory as the chlnpw script to avoid any errors.
If its your first time using it,then it might help to first run it using the -l option to learn more about the options available and the corresponding arguments.


You are free to use the program as you please,make modifications and distribute it as much as you want.
However,you can make a doantion by copy-pasting the link below onto your web browser.

https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=WX4B4KWEJJJJU&source=url

Any amount will be highly appreciated and will go a long way in supporting me and my work.





(C)2003 Dustin Spicuzza, Team 658
Complete 2003 code for our team
-----------------------------------------------------------------------------------------

FILES:

init.bsx		First slot program.. initializes bot
user.bsx		User control portion of code
joy1.bsx		Joystick recording control #1
joy2.bsx		Same file.. different name
joy3.bsx		..
joy4.bsx		..
project.rbe		RoboEMU project file
scratch.txt		list of scratchpad memory locations used
electric schem.doc	schematic for a 555 timer.. very simple. lacks values for RC though
readme.txt		This file

----------------------------------------------------------------------------------------

WARNING! THIS CODE PROBABLY WON'T WORK ON YOUR BOT UNMODIFIED.. DUH. YOU KNEW THAT I HOPE. 
USE CODE AT OWN RISK! IF YA KILL SOMEONE WITH YOUR BOT OR DO SOMETHING STUPID LIKE THAT
NEITHER I OR TEAM 658 OR OUR SPONSORS ARE RESPONSIBLE FOR THAT.. DEAL WITH IT. :-)

----------------------------------------------------------------------------------------

Notes:

#1: I use the new PBASIC syntax.. so have fun if ya dont have it

Here's what our code did for us:

3.5/4.5/5 Seconds to top of ramp in auto modes.. 
Very consistant auto modes, worked every time except for human errors. 
10th seed Great Lakes Regional, quarterfinals
Semi-finals Midwest Regional
9th seed West Michigan regional, quarterfinals

The strongest point about our bot is its autonomous mode.. period. It works consistantly
every time. 

Ok, you downloaded this code for no particular reason except you were bored and ya needed
something to do with your time. Well, since our team's season is over I am proud to release
our code from the 2003 season. This code is fairly well commented, here are just a few 
notes here from me.. 

-I used to use that timer a lot..  but I don't anymore cuz we got rid of a lot of extra
crap with we didn't need.. and so now it's only used for the joystick code. 

-I like using aliases a LOT. They are used extensively in the code, make sure everything is
correct.

-Umm... multiple slots.. you can figure out how to use those though. Its easy enough.

-In case you don't notice, our autonomous programs are selected using three switches.. 
essentially a binary encoder. Not too hard to teach your operator to use.

-Joystick recording stuff:
You need a time base of some kind.. timer is the varible to increment. Ours increments
timer every 1/10 second.. the input pulse is provided by the 555. Rather accurate time
base.. all the delays and crap are worked in there using that varible.. make sure it works or you're screwed.. lol. Also I have an invert switch, so we can go either left or right by switching the motor values around.. trust me, code is interesting.. study it. We just store
the motor values every 1/10 second, resolution is good enough to work very well. This code
could be modded quite a bit to have the stamp store up to 18-30 programs at once, but
that is quite unnecessary I think because of the presence of the invert switch. We actually
only used 4 stored programs.. and used only two regularly. Yeah.. just lots of stuff there.
Check it out. 

Well.. theres lots more, but you can figure it out probably. And if ya can't, email me at
randomperson83@hotmail.com and ask away.. my response time is usually within a day or so. 

-Dustin Spicuzza
randomperson83@hotmail.com

-Your perception is reality until you control it...

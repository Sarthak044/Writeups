# Academy
Heya people! So this is my first write up and I know there would be many write-ups of this particular machine/box, but it's first for me so bear with me here. 
If I miss something, kindly forgive me. So let’s get started without any further dangling.

So the box is Academy, I started this box during my course of PEH, by the way, awesome content, major shout out to heath Adams of TCM security, learned a lot from his course. You can find it here on the given link:
Practical Ethical Hacking - The Complete Course | TCM Security, Inc. (TCM-sec.com)
Just for context, I am using the latest parrot OS in a virtual box, don’t hate on me because I am not using kali. I booted the box and left it. First, let’s find out the IP of the machine we want to attack. So, like any other sane person, I ran a ping sweep in the network and didn’t find a thing. Yeah, not have a clue about IP. At first, I thought this box is blocking my pings, but it’s not Microsoft then why I am not getting an IP? After banging my head on my computer table I went back to the video and saw I had to run “dhclient” on the box after booting it up, solved the problem, phew! 
It showed up in the ping sweep, the command used was “Nmap -sn IP/CIDR”, easy. Now the fun part begins, Let's scan this bad boy and see what we are dealing with. I used basic Nmap scan, “Nmap -Pn -T4 -p- -v -A IP > nmapscan.txt&”, yup I didn’t use -On/-Ox or any other flag, I like to do a > scan.txt, it's kind of my go-to move, I don’t know why but I do.
Watched some awesome videos of networkchuck while the scan was doing the job, you can too.
![alt text](https://github.com/Sarthak044/Writeups/blob/main/imgs/watchit.jpg)
No pressure though.

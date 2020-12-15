Hour 1

**Hour 1**
**Again, these all go best with the slide deck provided**

If you want to work for BHIS, here are the things to know at base level.

This is meant to feed into various other BHIS trainings (Intro to Security, Purple Teaming, Cloud Breaching)

Today we are doing basic-level skills.  Some of you may be way more advanced, and that's OK.  respect both ends of the skill spectrum.

It will make you stretch a little bit in some areas.

John - with Department of the Interior
Certs are a huge barrier to getting started.  In order to address this, BHIS has created the courses.

------

People looking for jobs...
...jobs looking for people

Sometimes they are looking for the Golden Unicorn candidate.

--------------

Look at that 5-year plan, a video from BHIS.
You're gonna need to code, and have a code repository somewhere.

Feel like a SOC analyst currently drowning?  This course is for you.

So...today is a bad day for the Security Industry.  Solarwind popped, pushed to FireEye, malware.  Today (14 Dec) is a bad day.  Google services being down, is a little scary too.

**Why?**
*Slide 6*

Fear that action will lead to catasrophic failure.
You can absolutely interact with a compromised computer and network.  Just need to work with a plan.

Don't get into paralysis.

We have a 35GB VM.  We're going to work with something compromised.  Get your hands dirty.  You won't practice in the middle of a live-fire exercise.

The labs are all on Github, can open issues if there are typos, errors.

You can play around with the intro to security labs.

**The wrong way**
*Slide 7*

Developing detailed plans for everything.  Like, how to handle supply chain exploits.  Really? For Microsoft? For Solarwinds? For SSL Certs?  On and on...

Helmuth von Moltke the Elder — 'No battle plan ever survives contact with the enemy.'  Your detailed plan falls apart right away, then what are you stuck with?

**The Right Way**
*Slide 8*

Lego bricks.  Emmett the Lego Guy.
Backdoors and Breaches, blue procedure cards. Are basically the same as the Legos.
Things like Endpoint Analysis, Server Analysis, Internal Segmentation, UEBA

Every department is so dependent on flow charts.  "I'm so sorry"

**Don't Panic**
*Slide 10*

Keep Calm and Carry On.  Never posted during war.  Was planned for if England lost or was compromised.

Don't freak out, it is practice.  Like weapons trainings, practice again and again.  In different situations.  Not a "oh, here's a demo.  Can't see it again unless you pay more."

It is not, "Keep doing it until you don't do it wrong". Keep doing it until you **CAN'T** do it wrong.

Can build your runbooks around the markdowns in the labs.  Copy it, put your own logo on it, Strand doesn't mind.

**Endpoint Analysis**
Start with Windows
Not going into hard drive forensics.  That crap won't help you.  The remnants will be in memory or on the network.  Maybe at high levels, CSAM or Nation States.

Security Onion is a live VM environment that lets you do network-level forensics.

We will be doing memory forensics.

*Slide 12*

Difference between *knowing*, and just staring at a screen waiting for blinky lights to tell you things.

*Slide 13*

Core Windows Commands to know:
(maybe read the manuals for each one)
Netstat
net view
net use
net session

Netstat ...
netstat -naob
*See Slide 18*

Computer as a hotel with 65536 rooms.
Don't want netstat to make assumptions on what is behind that port. (This is what -n is for)
For things made by, in this example, PID 4, will get "can not obtain ownership information"  Because it was created by System
WinStore.App.exe ... who knows what M$ is sending out.

wmic to kill stuff. Not recommended to run.



Hour 2

**Hour 2**

Music of: fdisk, format, reinstall, doo-dah, doo-dah

What is the ASCII Buttcheek?[::]  It is IPv6

netstat -f
If cache poisoning is going, you will see it here

**Windows Processes**

NoScript is also handy to run to block ads
Blocking ads with OpenDNS or Cisco Unmbrella is fine, don't get too crazy.

**tasklist**
Horrible command in and of itself
By itself is junk, with no flags on it.
A solid name for malware is svchost.exe , because it will show up among multiple normal entries for svchost.exe

Looking at Task Manager.  Not giving a lot of IR perspective.

So extend tasklist with flags
tasklist /svc

Now you are getting more useful information
Still doesn't tell us "Is it evil?"

tasklist /m /fi "pid eq [proc_id]"
fi - filter

Like tasklist /m /fi "pid eq 3500"
*Slide 27*

You would think automated tools would do this.  They just don't do it all the time, they miss things.

-----------
Discussed in class:
https://www.darkreading.com/application-security/ransomware-makes-up-half-of-all-major-incidents/d/d-id/1339667?&web_view=true
"Yet attackers' capabilities improved as well. Cyberattacks were able to evade antivirus defenses in 40% of the incidents, and escaped notice in another 30% of incidents, **because the defender had misconfigured or failed to set up the antivirus correctly,**"

------------

PID is an identifier for processes in memory
If you notice our VM PIDs are diff than Strand's

We will be making it easier with Powershell and DeepBlueCLI
And yes, we will do a lab with it.

DeepWhiteCLI is sort of the next evolution.
It checks VirusTotal

--------
Lab, we're going to create malware

Become root

Run msfvenom

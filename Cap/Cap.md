# Cap - Writeup

Owned by `0x6ung3r`

We run a basic nmap scan:

![[Pasted image 20260830213813.png]]

We check out the website:

![[Pasted image 20260830214201.png]]

We check out the Security Snapshot menu:

![[Pasted image 20260830214309.png]]

We notice that there is a potential IDOR vulnerability in the link. We can try and fuzz this, or just quickly change the 1 in the link with different values and see what happens. It looks like changing it to 0 displays the PCAP of another user:

![[Pasted image 20260830214629.png]]

This seems promising. Let us download the pcap.

From our nmap scan earlier, we remember that there is also an ftp server lying around. What if we can find the password in the pcap we just downloaded, since FTP traffic is in plaintext?

We open the pcap in Wireshark and filter for FTP traffic. The password pops up immediately:

![[Pasted image 20260830215315.png]]

We use the username and password we found to login to the FTP server:

![[Pasted image 20260830215549.png]]

From there we can download the user.txt for the flag.

These credentials turn out to work to login through ssh as well. 

![[Pasted image 20260830220105.png]]

Now let us find a way to elevate our privileges. First thing I tried is to enumerate the SUID set binaries using `find / -user root -perm /4000 2>/dev/null`, but nothing stood out:

![[Pasted image 20260830221158.png]]

Since the machine is called Cap, let us use `getcap` to get the capabilities of all of the files in the file system. We can do this using `-r`:

![[Pasted image 20260830221341.png]]

And we found a version of python with the `cap_setuid` capability. Using GTFObins, we can easily take advantage of this:

![[Pasted image 20260830222055.png]]

And thus we are root.


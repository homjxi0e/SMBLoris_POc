# what IS the Smb !! 
Me sharing files remotely by Protocol SMBv1 Or SMBv2 SMBv3 
-------------------------
vulnerable On Next in Text from i,am 
The vulnerability is in all modern versions of Windows, at least from Windows 2000 through Windows 10. Systems are still vulnerable even if all versions of SMBv1 SMBv2 SMBv3 are disabled

It is computationally inexpensive for an attacker to cause large memory allocations and enormous amounts of wasted CPU cycles†, rendering vulnerable machines completely unusable, making business-critical services (such as web and mail servers) unavailable, and even causing the entire operating system to crash !!
''''''''''
And Windows immediately commits in memory a number of bytes determined by the attacker-controlled Length field, which is 217 for a max of 131,072 bytes (128 KiB). This memory is in the "non-paged pool" (physical RAM) which cannot be swapped out to disk, making the denial of service even more effective. CPU and memory resources are effectively lost for as long as the connection is sustained

------------------------------------------------------------------------------------------------------||
------------------------------------------------------------------------------------------------------||
"SMBLoris works over IPv4 and IPv6, and acquiring multiple IPs on a LAN can amplify the attack. The amount of machines required to perform a distributed denial of service (DDoS) attack against more powerful servers is also significantly reduced.
=

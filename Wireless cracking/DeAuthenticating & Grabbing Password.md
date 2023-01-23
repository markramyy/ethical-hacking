# DeAuthenticating & Grabbing Password
---

- ###  We will put the Wireless Card on [[Monitor Mode]] , we don't want to sniff all of the information around us so we need to pick the one we want to Attack.
---
- ### Once we choose our target, we need to check out the Channel on which the Target is running on and it's Mac Address.
---
- ### Then running our sniffing program and simultaneously we must run our #DeAuthentication Attack.
---
- ### That will make the devices to  disconnect from the Access Point for a few seconds and once we stop it, we should be able to sniff the #FourWayHandshake with the Hash Value of the Password.
---
 - ### So How we actually do that :

1. First step you need to make sure that your Wireless Card is in #MonitorMode .
---
2. After that you run a built-in Program inside of Kali : **airmon-ng check {Wireless Interface}** 
![[airmon-ng check.png | 600]]
---
3. It will tell you that it found a number of processes that could cause some trouble during our process of gathering the #FourWayHandshake with the password.
---
4. So we don't want to take the risk, we will kill all of these processes using :  **airmon-ng check kill**.
![[airmon-ng kill.png | 400]]
---
5. Then you just need to check if your card is still in #MonitorMode since it sometimes turns back to management.
---
6. After that we need to see the available Access Points and its information in our area so we run the code :  **airodump-ng {Wireless Interface}**.
![[airodump.png | 600]]
---
7. Just choose your Target Network's name(ESSID) and you need to remember the Channel number and the Mac-Address to preform the Attack.

8. We need to start the sniffing process, however we're going to write information inside of a file.
---
9. we use the command : **airodump-ng -c "channel num" --bssid "Mac Address" -w "file name" {Wireless Interface}**.

![[airodump code.png | 600]]

---
10. You need to make sure to remember on which destination are you running the command because that is where it's going to save your files.

11. We can't wait until someone tries to connect to this network so we need to preform the #DeAuthentication Attack to kick everyone out of the network.
---
12. To do that we run the command:
				**aireplay-ng -0 0 -a "Mac Address " {Wireless Interface}**.      
	PS: The Mac-Address of the target.
![[De-Authentication 1.png | 600]]
---
13. This is a lot of steps but after that when someone tries to reconnect to the network you will be able to catch the handshake 

![[Handshake.png | 600]]

---
14. So now you got everything you need that's the #FourWayHandshake  that contains the password 

15. Once you finish you will find a multiple files on your destination, we actually only need one file that with the extension **.cap** and inside of it is the handshake that we just got.
---
- ### After that we are going to use different tools to extract the hash password from this .cap file and use a massive word lists to try to crack this password, Like [[AirCrack]] and [[HashCat]]. 
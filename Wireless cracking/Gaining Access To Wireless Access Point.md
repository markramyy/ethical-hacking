# Gaining Access To Wireless Access Point
---

- #### This process can be complex because it requires a lot of Tools to complete. Besides Tools, it also requires something that you might or might not have, that's a Wireless Card that supports [[Monitor Mode]].

---
- #### Monitor Mode allows us to Sniff Data from Access Points around us, which then we  will use to sniff the #Hashed Password once someone tries to connect the Wi-Fi.

---
- #### Your device isn't connected to the Wireless XPoint, it only has to be close to preform this Attack. Once we get close to Our wireless AP, we turn our Wireless Card into Monitor Mode.

---
- #### Once we have it in #MonitorMode, we will be able to see all of the Wi-Fi around us as well as our Target, when we choose out of all those Access Points, which one we want to Attack, we need to Identify two things about that Access Point.
			1. The **Channel** on which it runs (3).
			2. It's **Mac Address** (FA-45-63-89-EF-13).

---

![[Wireless Access Point.png | 600]]

---


- ### How can we Catch the Password:

1. Once it tries to connect to that Wireless Access Point, it will initiate Four Different Steps, also known as a #FourWayHandshake between the device and the Access Point.
2. In those Four Steps, it sends the Password value to the Access Point, and that what we want to Sniff.
---
3. However, it could take a long time until someone tries to connect to that Wi-Fi. So we are going to preform a different type of the attack to kick everyone off of the Wi-Fi, that's called [[DeAuthenticating & Grabbing Password]] Attack.

4. Once we send it's packets, this will disconnect every device that was previously connected to the Access Point.
---

![[De-Authentication 1.png | 600 ]]

---

5. When that happens, every device will try to reconnect to the Access Point and all that time we will be sniffing for that four way Handshake with our password key. 

6. Once they connect, we will get the password value that we want.
---
 
![[Hashed-Pass.png | 600]]

---

7. Then we will throw this Hashed Password into different tools that can help us crack this Password.
		i) [[AirCrack]] that uses CPU Power or Processor Power to crack it.
		ii) [[HashCat]] can use both CPU or Processor Power and your Graphics Card Power. And sometimes it crack a lot faster than AirCrack.

8. The Average Speed of cracking password with these programs, depend on what CPU and GPU you have, would be around 300->100000 Passwords per Second.
---

![[Crack-tools.png | 600]]

---

- #### So this is a completely different story than, for example, brute forcing weblog and Page or SNH or something similar. It is a lot faster.

- #### If the Password is not complex and we managed to crack it. We can connect to that far less Access Point, and if we want we can attack the devices inside that Network with all the previous Attacks that we learnt.

---

![[Attack the wireless.png | 600]]
# HashCat
---

- ### Here we crack the password using both CPU or Processor Power and your Graphics Card Power, that what makes it a lot faster than AirCrack.
---

- ### We will use the same #rockyou text file that we used earlier. If you can't find it just re-do the steps that we used on [[AirCrack]].

- ### Do not forget to put your Wireless Card on #MonitorMode.

---

- ### Hashcat has a lot of option to be considered from the different type of Hashes, different attack mode and device type, etc...

- ### You just need to run the command : "hashcat --help" and it will display all the various option that we have.
---

![[hashcat option.png | 600 ]]

---

![[Attack mode.png | 600]]

---

- ### After that you need to choose the type of hash that you will attack {WPA2} and the attack mode.

![[hashcat help.png | 600 ]]

---

- ### And that's how you begin the hash :

1. First of all the hashcat doesn't work with the **.cap** file so you need to convert it to **.hccapx** file to make it work.

2. You do that using any online converter like { https://www.onlinehashcrack.com/tools-cap-to-hccapx-converter.php } and covert your hash file to the right extension
---

![[online covert.png | 600 ]]

---

3. After you do that type the command : 
			**hashcat  -a  "attack mode" -m "hash number" "file.hccapx" rockyou.txt**

![[hashcat command.png | 715 ]]

---

4. Then it will display some information about the device and the hash file.

![[hashcat device info.png | 600 ]]

---
5. Finally it will begin the Hashing.

![[hashcat crack.png | 600 ]]

---
- ### There are a lot of tools that can be used other than these like {wifite , airgeddon , kismet ,etc... } .

- ### you just need to search for them and to figure out how they operate .

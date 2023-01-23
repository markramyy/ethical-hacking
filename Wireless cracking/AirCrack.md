# Air-Crack
---
- ### Here we crack the password using CPU Power or Processor Power to crack it.

- ### Now after we obtained the #Hashed Password and copied it in a file with the extension .cap, we will use it to crack the Password.
---
- ### Unlike any other #BruteForce tag that we previously did with small password lists of tens or hundreds or thousands of passwords.

- ### This is going to be a huge password list, it contains over 10 million unique passwords and it's on Kali linux machine called #rockyou text file.
---

- ### So how you can find it, just run the command : 
### 						" locate rockyou.txt " 

![[Location rockyou.png | 700 ]]

- ### It will let you know the location of the file that contains the list of passwords.
---
- ### So what do we do next : 

1. After that you change the directory using **cd** command to the location of the list. And copy it **cp** and paste to an easy location so that you can use it later.

---
2. it will be a zip file with the **gz** extension so we just need to unzip it using this command : 
				             		**gzip  -d rockyou.txt.gz**

![[rockyou gz.png | 700 ]]

---
3. If we actually tried to **cat** this file, you will see that the list is just keep displaying and go on forever.  

4. But you can actually control by adding some changes and add some passwords it using **nano** command, it will take a couple of seconds to load because the content of the file is too big.
---

![[rockyou txt.png | 700 ]]

---

5. Now we just need to combine **rockyou file** with the **.cap file** using the **aircrack** tool using the following command :
						**aircrack-ng  -w  rockyou.txt  "file name.cap"**

![[Aircrack command.png | 700 ]]

---
6. After that you sill see that it's start cracking our password. And you wait until it finds the password or when the estimated time end or the process percentage is 100%.

![[Aircrack-ng.png | 700 ]]

---

- ### Keep in mind that the speed differs from a virtual machine to laptop to a built-in computer. It all depends on the Hardware and the capabilities of the device that you are preforming the crack.

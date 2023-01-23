# Monitor Mode
---

- ### You need this Wireless Card to perform an Attack on a Wireless Network's Access Point.

- ### That's how we use It:
---
1. You must type the command : **ifconfig** to find your interfaces names and info.

![[ifconfig.png | 600]]

---
2. then type : **iwconfig** to figure out what is your wireless card.
![[iwconfig.png | 600]]
---
3. We need to change the mode of the card "Managed" to #MonitorMode, you need to do a list of commands in order to do so.

4. First we need to type : **ifconfig {Wireless Interface} down**, Second : **iwconfig {Wireless Interface} mode monitor**, Last :  **ifconfig {Wireless Interface} up**

5. After you finish to double check type : **iwconfig** and you will see it changed into Monitor mode.
---

![[Monitor Mode.png | 600]]

6. if you discover that it returned to the Managed Mode don't worry you just need to preform the same steps multiple time.
---
- ### And that's the First Step you need to preform to begin any kind for Wireless Attacking.

- ### Second Step is the [[DeAuthenticating & Grabbing Password]] and we will talk about it in much detail later.


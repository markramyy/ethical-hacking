# Information Gathering & Reconnaissance
---

- ### **It is the first step in Penetration Testing and an Act of Gathering data about our Target.**

- ### **It can be any type of data that we might find useful for the Future Attack**...

---

### 1. #Active *Information Gathering* :

- #### We try to get as much Data or Info while interacting with them. It could be a target Website that we need to test or a Network that we are testing or perhaps an entire Company.
---
- #### The main point is to directly get the data from the target. This could mean directly exchanging packets with the target visiting and Enumerating their Website or mean talking to employee works there {it's considered Social Engineering}.

- #### It provides us with more important Data than passive Information Gathering since we are directly interacting with the target.

---

### 2. #Passive *Information Gathering* :

- #### It is Information Gathering using a Middle Source (Intermediate System) and it could be anything from Search Engine to Website to Person.
- #### If you search on Google that target to find some pages that contains information about it, It's considered a passive Information Gathering.

---

### 3. *Obtaining IP Addresses*:

#### 1) #Active : Interact with the target directly.

- Using **Ping** " Website-name ", we are sending something called ICMP Packets to the Website and if we get responses back then that website is up and running.

![[Ping.png | 700]]

---

- Using ** nslookup ** " Website-name "

![[nslookup 1.png | 500]]

---

- **whois** " Website-name ". That will bring back a lot of information including IP address, actual address, deployment, etc...

![[whois.png | 700]]

---

- **Red Hawk** using this tool with php files to get information about any Website.
![[RedHawk.png | 700]]
---
![[RedHawk2.png | 700]]

---

- **Sherlock** using it with python3 to obtain data about Usernames through Websites and Links.
![[sherlok.png | 700]]

---

#### 2) #Passive :

- Using Anther website Like ( ipinfo.info ).

![[ipinfo.png | 700]]

---

### 4. *Whatweb Tool* :

- #### It is used to gather information and scan any Website on the Internet that has a lot of Plugins that is used to recognize something different and also Identifies version number, email addresses, Account IDs, Web Framework Modules, SQL Errors and more.
---
- #### The Default Level of Aggression is called "Stealthy" is the fastest and requires only one HTTP request of a Website. It's suitable for Scanning public Websites.
---

- #### **More Aggressive Modes were Developed for use in Penetration Tests ( Need Permissions!!! )**.

![[whatweb 1.png | 700]]

---



# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/e08c8a3a-2c67-4ac4-8951-87c6b3e0e1e3)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/8066e7f0-535b-4f0b-b26c-0264566aa9a8)
intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/43f66d44-8202-4d82-8595-94719c5b0562)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/6a781cb2-033e-4e54-9acd-81daa4d272c0)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/8654dbf2-6ef1-4a74-af82-e4541222c472)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/6023dae5-89b0-428f-962b-fb4f6edf62b6)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/d1216b10-b1f3-4729-a79a-885558d04249) 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/93bab85a-b811-4b26-b82c-873386e8c57d)
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/125c2132-c513-40b0-8cf7-61a27b77c810)


##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/cfdbd280-31d2-402e-bb9c-4f70c560ba0a)
##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![n](https://github.com/praveenst13/Enumeration/assets/118787793/d8415f64-ebd0-4eb9-a4e8-002f220f4f91)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![Screenshot 2023-05-22 134841](https://github.com/praveenst13/Enumeration/assets/118787793/6257b51a-4fdc-44cc-aaba-cdca76d7f4e5)

select any username in the first column of the above file and check the same
![o](https://github.com/praveenst13/Enumeration/assets/118787793/5d8df46a-e4c3-4b86-884d-6e01014da92a)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  ![p](https://github.com/praveenst13/Enumeration/assets/118787793/42446d0a-0057-47dd-8d50-f3ea43a5e632)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/vishnudorigundla/Enumeration/assets/94175324/a3c19d91-14c5-4648-a863-dea7a9470eb1)
## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

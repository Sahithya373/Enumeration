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
## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/9ba4165d-b8a2-49db-b271-42e899d93ae6)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/3c6a9993-bb40-4696-ba36-d0673c47ad52)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/ac2dfe0c-41c4-4c05-a797-52470cc2a3a1)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/9208b138-27a5-4ce7-ad4e-2aebe99bed21)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/2b468473-464a-44f0-8b28-815d6b23a933)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.


## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/57cd1703-4643-4887-93fb-5a06aa2d6e36)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/6fb0cbca-2c35-411e-b2f6-711ab091021a)


 
#DNS Enumeration

##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/2ed47124-92c3-479d-b006-1521057b3792)


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

![image](https://github.com/Sahithya373/Enumeration/assets/147017926/af1466e8-04f4-49ef-bcd0-6f09e76ef7a8)

![image](https://github.com/Sahithya373/Enumeration/assets/147017926/6149d9ce-f490-4fdf-b2d7-cf154d5cfaf6)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![image](https://github.com/Sahithya373/Enumeration/assets/147017926/a35f8106-520c-406a-9913-99c729c6f7c6)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![image](https://github.com/Sahithya373/Enumeration/assets/147017926/71bf904a-da66-4b89-b0b3-e737677ca750)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## OUTPUT:
 ![image](https://github.com/Sahithya373/Enumeration/assets/147017926/76eee789-4615-4e24-bad9-3bb35ba82fa5)

  
 ## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
![image](https://github.com/Sahithya373/Enumeration/assets/147017926/df55d031-ca07-406b-a690-38e553c7ae9a)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully


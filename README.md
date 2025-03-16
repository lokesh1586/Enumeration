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

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com


![Screenshot 2025-03-16 150510](https://github.com/user-attachments/assets/273aef04-83fb-48dd-af18-9302e8a393e2)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![Screenshot 2025-03-16 150638](https://github.com/user-attachments/assets/9bb1aea6-20c1-4873-b06d-0b1816a93a8e)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![Screenshot 2025-03-16 150745](https://github.com/user-attachments/assets/06f2b86d-598b-4d99-93ba-b37705309bfc)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![Screenshot 2025-03-16 150839](https://github.com/user-attachments/assets/9f0b4e6e-74fd-4a95-b12f-019911a02270)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![Screenshot 2025-03-16 150953](https://github.com/user-attachments/assets/7b203887-b7d1-4c0d-a935-94a1bcd9c719)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 ![Screenshot 2025-03-16 151126](https://github.com/user-attachments/assets/6409822a-f174-4b05-b1b7-7c61a6492d5f)
![Screenshot 2025-03-16 151232](https://github.com/user-attachments/assets/62021925-0302-48b6-bffc-d63e36e0b753)

#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![Screenshot 2025-03-16 143419](https://github.com/user-attachments/assets/e3e8c6df-c4bf-4bd8-a0c8-d9cdda5929ac)

![Screenshot 2025-03-16 143603](https://github.com/user-attachments/assets/494a968f-4989-436c-aad4-0cb3c3391887)





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

![Screenshot 2025-03-16 143945](https://github.com/user-attachments/assets/8229d4e1-199a-4dd3-8767-d1bdfed82a1d)
##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![Screenshot 2025-03-16 145713](https://github.com/user-attachments/assets/d79f5712-4d31-4636-8914-65a2c4b601d6)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![Screenshot 2025-03-16 145724](https://github.com/user-attachments/assets/561f93d0-b1de-4d68-9e07-76420c5295a3)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Screenshot 2025-03-16 145807](https://github.com/user-attachments/assets/5cf52b48-6729-4cd8-84a3-c75aa507df99)
![Screenshot 2025-03-16 150049](https://github.com/user-attachments/assets/20f89b41-0e9f-4c18-a59c-974f309de051)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully


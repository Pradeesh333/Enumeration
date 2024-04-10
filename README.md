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

![image](op1.png)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## OUTPUT:

![image](op2.png)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## OUTPUT:

![image](op3.png)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## OUTPUT:

![image](op4.png)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## OUTPUT:

![image](op5.png)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## OUTPUT:

![image](op6.png)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## OUTPUT:

![image](op7.png)

# DNS Enumeration

## DNS Recon

provides the ability to perform
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:

![Screenshot from 2023-05-22 04-42-40](https://github.com/22003264/Enumeration/assets/119389139/404a97fc-30d3-4dbf-bd44-e87e8a6a7c4d)

![Screenshot from 2023-05-22 04-39-59](https://github.com/22003264/Enumeration/assets/119389139/cccb27a8-2711-492a-bda9-5fa261c0f27c)

## dnsenum:

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

## OUTPUT:

![Screenshot from 2023-05-22 04-51-50](https://github.com/22003264/Enumeration/assets/119389139/2c7f0da3-b169-4390-a802-e7da5842a787)

## smtp-user-enum

Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![Screenshot from 2023-05-22 04-59-45](https://github.com/22003264/Enumeration/assets/119389139/36268e62-becc-4a52-971d-0db0460b9673)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![WhatsApp Image 2023-05-22 at 14 47 12](https://github.com/22003264/Enumeration/assets/119389139/2decc652-0645-4faa-a05d-aee0d3903515)

select any username in the first column of the above file and check the same

![Screenshot from 2023-05-22 05-01-29](https://github.com/22003264/Enumeration/assets/119389139/213e9b42-33e5-41d4-a2bc-ec3e7c03bd72)

# Telnet for smtp enumeration

Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

![Screenshot from 2023-05-22 05-17-08](https://github.com/22003264/Enumeration/assets/119389139/6c49d93b-c710-4e51-87af-d6cb5a453918)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

![Screenshot from 2023-05-22 05-26-00](https://github.com/22003264/Enumeration/assets/119389139/5a15bf55-ccc2-4c84-81bc-a7975acc0265)

## RESULT:

The Google hacking keywords and enumeration tools were identified and executed successfully

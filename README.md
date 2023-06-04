## The Time Machine - Weaponizing WaybackUrls for Recon, BugBounties , OSINT, Sensitive Endpoints and what not

![TimeMachine]

### Introduction 

Inspired by anmolksachan

I have updated this tool for making my work easier when it comes to recon and fetching sensitive endpoints for sensitive data exposure and further exploitation using waybackurls and sorting for Sensitive endpoints, it has also option  to look for sensitive endpoints for information disclosure, It has have more capabilities like looking for possible endpoints vulnerable to XSS, LFI, JIRA Based Vulnerability, Open Redirection.

I'm not too much into bug bounty but recently gained interest and leaarning a lot.

It worked on multiple bug bounty program, reports are still under review.

### Features

1. Search for /api/ endpoint
2. Search for JSON endpoint
3. Fetch possible Conf(configuration) endpoint
4. All Possible Sensitive instances in URL from TheTimeMachine (Searches from Fuzz List) or can also Add your own Custom List
5. Fetches subdomains from waybackurl
6. Search Custom keyword of your choice Eg. backup, .log etc.
7. Attack Mode ( Searched for vulnerable possible endpoints for SQLi, LFI, XSS, Open Redirect, Wordpress, JIRA Based Vulnerability or via Custom File, PS More to be added soon )
8. Fetch only Parameters from any file (Eg. Fetched from way back urls, extracted file from Attack mode or any URLs file, also how creative you are can be used with burp spider file :P) 
9. You can manually edit all the files that searched for XSS, LFI, Fuzz etc.

### How to install and use 

Note : Tested with python3 on Ubuntu/Kali/Windows

```
$ git clone https://github.com/Tron-o/WaybackUrls
$ cd WaybackUrls
$ pip3 install -r requirements.txt
$ python timemachine.py

```

If you're not able to install requirements.txt, run install.sh or install manually, run below mentioned commands

```
$ pip install numpy
$ pip install requests
$ pip install colorama
$ pip install termcolor

```

Example Run : 

Note : Entered URL must look like domain.com or subdomain.domain.com no http or https is required

```
$ python timemachine.py domain.com
$ python timemachine.py subdomain.domain.com
.. .. .. .. 
.. .. .. .. 
AND SO ON 

```
![enter image description here](https://raw.githubusercontent.com/Tron-o/WaybackUrls/main/run.PNG)

### Add your own list of payloads

```
you can edit multiple available payloads and Fuzz , 
Add your own in the interested text file !

```

### Special Thanks For making such a great Tool

[Anmol K Sachan](https://github.com/anmolksachan)

## __Want to support my work?__
Give me a Star in the repository thats enough for me.

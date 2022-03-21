# Ngnix Virtual Hosts

For demonstration purposes were created three apps examples:
- site1: whose assets files use root absolute path
- site2: whose assets files use relative path
- site3: sample of SPA (build of react app) 

Note: assets folder was placed on same level of apps to illustrate calls to root domain.

## Question
Can multiple sites (can be SPA too) be on the same domain?
### 1. Based Name Approach

For this method work, it's needly edit `hosts` file.
 - for based unix system: `/etc/hosts`
 - for windows system: `c:\Windows\System32\Drivers\etc\hosts`

 Add the following instructions:
 > 127.0.0.1 site1.local  
 > 127.0.0.1 site2.local  
 > 127.0.0.1 site3.local

Nginx configuration: `based-name.conf`

### 2. Based IP Approach

Nginx configuration: `based-name.conf`

uygroa
=============
Welcome to uygroa, a DNS based ad blocker forked from ublockr. uygroa redirects ad domains to pixelserv-tls webserver.
Requires entware + usb storage mounted to router

Requirements
--------------
* Router with entware capabilities
* A swap enabled USB drive mounted to the router

Installation
--------------
1. wget https://raw.githubusercontent.com/Knapoc/uygroa/master/uygroa -O /opt/bin/uygroa --no-check-certificate
2. wget https://raw.githubusercontent.com/Knapoc/uygroa/master/uygroa.cfg -O /opt/etc/uygroa.cfg --no-check-certificate
3. chmod +x /opt/bin/uygroa
4. Run it periodically with cron... e.g: 0 0 * * * /opt/bin/uygroa

The configuration is done in **/opt/etc/uygroa**

Additions to the original ublockr
--------------
* Compatibility with malware-filter (https://gitlab.com/swe_toast/malware-filter) by Toast
* Compatibility with privacy-filter (https://gitlab.com/swe_toast/privacy-filter) by Toast
* Clear cache function
* Update host file sources (listupdate)
* Option to disable whitelists

Options
--------------
* **-update**

   updates uygroa with the latest github version
* **-version**

   shows version number
* **-listupdate**

   deletes ip.list and no.list and downloads them again from github. ip and no ip lists contain the sources for the host file.
* **-clearcache**

   deletes all lists (incl. whitelist)

# uygroa
DNS based ad blocker forked from ublockr featuring Pixelserv-TLS

Requires entware + usb storage mounted to router
Installation:
1. download the files to your desired directory.
2. change the config file's path in uygroa (line 48)
3. Run it periodically with cron... e.g: 0 0 * * * /opt/bin/uygroa

Additions to the original ublockr:
* compatible with malware-filter & privacy-filter by Toast
* clear cache function
* update host file sources (listupdate)

Options:
* -update
    Updates uygroa with the latest github version
* -version
    shows version number
* -listupdate
    deletes ip.list and no.list and downloads them again from github. ip and no ip lists contain the sources for the host file.
* -clearcache
    deletes all lists (incl. whitelist)

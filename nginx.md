# nginx

## Config

* /var/log/nginx directories should be owned by root:root and have permissions
  (at least?) 755 to mitigate CVE-2016-1247:
  https://legalhackers.com/advisories/Nginx-Exploit-Deb-Root-PrivEsc-CVE-2016-1247.html

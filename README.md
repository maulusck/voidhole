##### VOIDHOLE DOCUMENTATION #####

 - MAIN ISSUES:
 
 - script is configured for systemd
	- systemctl -> sv, i.e.

 - IP settings totally fucked up, be better to set it up manually
	- need manual config in setupVars.conf
 
 - pihole-FTL binary (musl)
	- checksum verification fails and force reinstall
	- musl is not within the default options -> download manually
	- 

 - lighttpd + PHP
	- not enabled by default
	- missing php-cgi
	- need conf in conf.d/cgi.conf
	- need modules enabled
	- 
	
 - php exec() sudo pihole needs full path [/usr/local/bin]
	- added command log to pihole-cmd.log in func.php [chown _lighttpd]


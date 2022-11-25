# Apache 
1. Install apache2(Ubuntu) or httpd(CentOS). 
2. Edit /var/www/html/index.html file or you can put free site templates.
3. Start apache service and open this service to others using firewalld.
4. Try to open your site from Windows google chrome. http://ipaddress
5. Open /var/log and open access_log file, read the output of it.

# DNS
1. After configuring Apache webserver, install bind-utils bind packages(CentOS), and start configuring DNS server.
2. When you finished configuring check that your DNS works with the command 'nslookup test.site.kg'(you can choose different domain name) or 'nslookup 192.168.0.?'. Or you can curl -k https://Domain name, instead of an IP.
3. If you want to access from Windows web browser, Open ControlPanel/Network and Internet/Network Connections and change the properties of an Ethernet --> Open Internet Protocol Version 4(TCP/IPv4), Preferred DNS server: should be the IP of your Virtual machine IP. Alternate should be the 8.8.8.8
4. Now you can access from your web browser by typing Domain name instead of and IP address.
5. After completing steps above switch back DNS priority in your Windows OS.

# HTTPS SSL
1. Add free certificate to your website and type in your browser,example: 'https://test.site.kg'. It should open your site, but since it is free certificate google chrome will show warning page, just skip it and open.

# Note
1. When you are working with https, allow its port or service.

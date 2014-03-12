wowza-nginx-template
=====================

Description
-----------

This is a minimal template to get info about your NGINX server.

Monitoring information by now:

* active
* accepted
* handled
* requests
* reading
* writting
* waiting


Install
-------

You should look for the external scripts directory in your Zabbix configuration file. 
In the CentOS 6.4 RPM Zabbix installation is: 

``` 
 /usr/lib/zabbix/externalscripts 
```

Copy the python script there. A chmod/chown to get execution permission is necessary.

Now, in your Zabbix frontend: Configuration-Templates section, Import bottom in the right.

Choose the XML file and import.

Apply this new template to your Wowza servers. 

You don't need to modify the template if you are using the standard port to access to the Wowza URL (port 8086).

Environment
-----------

I am using this script in my production environment:

* Nginx 1.4.5
* Zabbix 2.2.x


TODO
----

* Zabbix template pending, this a first release.

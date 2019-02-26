Zabbix template apcupsd
==========================
Based on https://github.com/cavazquez/zabbix_template_apcupsd

Specified for Smart-UPS 1500

Tested on Zabbix Version 4.0

Should work on 3.2

FEATURES
--------
* Model
* Driver
* Metrics set in __apcupsd.conf__:
  * Min battery charge required for system shutdown
  * Min battery runtime required for system shutdown
  * Max battery runtime after which system is shutdown
  * Input, output and battery voltage
  * Battery charge
  * How long host will hold on with batteries
  * Temperature
* Status Connection
* Alert on no minimum charge shutdown is set
* Alert on low input voltage
* Alert on low battery charge
* Alert on high temperature


REQUIREMENTS
------------
* Zabbix server version 3.2

INSTALLATION
------------
* Agent
  * Install and configure apcupsd daemon
  * Copy __apcupsd.conf__ to __/etc/zabbix/zabbix_agentd.conf.d/apcupsd.conf__
  * Restart zabbix_agent
* Server
  * Import template __template_apcupsd.xml__ file


LICENSE
-------
GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007

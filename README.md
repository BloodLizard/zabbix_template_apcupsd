Zabbix template apcupsd
==========================
Based on https://github.com/cavazquez/zabbix_template_apcupsd

Tested on Zabbix Version 4.0

Should work on 3.2

FEATURES
--------
* Model
* Driver
* Shows the set in __apcupsd.conf__:
  * MBATTCHG: Min battery charge % (BCHARGE) required for system shutdown
  * MINTIMEL: Min battery runtime (MINUTES) required for system shutdown
  * MAXTIME : Max battery runtime (TIMEOUT) after which system is shutdown
* Status Connection



REQUIREMENTS
------------
* Zabbix server version 3.2

INSTALLATION
------------
* Agent
  * Copy __apcupsd.conf__ to __/etc/zabbix/zabbix_agentd.d/apcupsd.conf__
  * Restart zabbix_agent
* Server
  * Import template __template_apcupsd.xml__ file


LICENSE
-------
GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007

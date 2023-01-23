# Template App Elasticsearch Cluster by Zabbix agent

## Overview

For Zabbix version: 5.0,6.0 and higher. 

These templates are based on the "Zabbix agent" version of the HTTP template shipped with Zabbix 5.0/6.0 (https://www.zabbix.com/integrations/elasticsearch)
This version can connect to elasticsearch on localhost or a remote network using the zabbix-agent. (does not use simple checks!)
The metrics are collected in one pass remotely using `web.page.get` and HTTP/HTTPS

This template was tested on:

- Zabbix, version 5.0, 6.0
- Elasticsearch , version 6.x, 7.x

Additionally to the original Zabbix template:
* The indices are checked for read-only status.
* The `cluster_name` item is collected from node stats.

## Zabbix configuration

No specific Zabbix configuration is required.

### Macros used

Please read the descriptions in the template.

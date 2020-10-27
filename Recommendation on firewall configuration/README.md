This article explains how to configure a firewall for network connectivity when users want to use the SDK (especially the browser-based SDK) behind the firewall.

## Requirements for Signal Connectivity
|Protocol|Behind firewall<br>Source IP&nbsp;&nbsp;&nbsp;Source Port                     |Allowed destinations<br>Wildcard FQDN*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Port|
|:------:|:-----------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------|
|TCP     |ANY&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ANY|*.calls.sendbird.com&nbsp;&nbsp;&nbsp;443                                                            |

*If you cannot use wildcard FQDN as the destination address, set it to ANY.
 
> If you need a static IP list, please go to your dashboard and file a ticket.

## Requirements for Media Connectivity when using Direct Call
|Protocol|Behind firewall<br>Source IP&nbsp;&nbsp;&nbsp;Source Port                     |Allowed destinations<br>Wildcard FQDN*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Port|
|:------:|:-----------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------|
|UDP     |ANY&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ANY|*.calls.sendbird.com&nbsp;&nbsp;&nbsp;5349                                                           |

*If you cannot use wildcard FQDN as the destination address, set it to ANY.

> Static IP list is not provided for connectivity to Media Server.

## Requirements to enable direct P2P connection with STUN
|Protocol|Behind firewall<br>Source IP&nbsp;&nbsp;&nbsp;Source Port                     |Allowed destinations<br>IP address&nbsp;&nbsp;&nbsp;Port|
|:------:|:-----------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|UDP     |ANY&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ANY|ANY&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1024-65535|


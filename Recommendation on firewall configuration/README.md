This article recommends how to configure firewall for a network connectivity where the service works well when users use the SDK (especially the browser-based SDK) behind the firewall.

<br><br>
## Requirements for Signal Connectivity
|Protocol|Behind firewall<br>Source IP&nbsp;&nbsp;&nbsp;Source Port                     |Allowed destinations<br>Wildcard FQDN&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Port|
|:------:|:-----------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------|
|TCP     |ANY&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ANY|*.calls.sendbird.com&nbsp;&nbsp;&nbsp;443                                                            |

> If you cannot use wildcard FQDN as the destination address, set it to ANY.
 
> If you need a static IP list, please contact @??who. Additional charges may apply.

<br><br>
## Requirements for Media Connectivity when using Direct Call
|Protocol|Behind firewall<br>Source IP&nbsp;&nbsp;&nbsp;Source Port                     |Allowed destinations<br>Wildcard FQDN&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Port|
|:------:|:-----------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------|
|UDP     |ANY&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ANY|*.calls.sendbird.com&nbsp;&nbsp;&nbsp;5349                                                           |

> If you cannot use wildcard FQDN as the destination address, set it to ANY.

> Static IP list is not provided.

<br><br>
#### To enable direct P2P connection using STUN, set as follows
|Protocol|Behind firewall<br>Source IP&nbsp;&nbsp;&nbsp;Source Port                     |Allowed destinations<br>IP address&nbsp;&nbsp;&nbsp;Port|
|:------:|:-----------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|UDP     |ANY&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ANY|ANY&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1024-65535|


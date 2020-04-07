# A lightweight shipper for forwarding and centralizing log data. 

Installed as an agent on your servers, Filebeat monitors the log files or locations that you specify, collects log events, and forwards them to your Vizion.ai elasticsearch instance.

## Installation:

#### <b>Option 1.</b> Automated Installation.

### Windows:

1. As administrator, enter the following command in Powershell or download the zip file [here](https://github.com/themarcusaurelius/Filebeat/archive/master.zip).

```
Start-BitsTransfer -Source 'https://github.com/themarcusaurelius/Filebeat/archive/master.zip' -Destination 'C:\Users\Administrator\Downloads\filebeat.zip'
```

# A lightweight shipper for forwarding and centralizing log data. 

Installed as an agent on your servers, Filebeat monitors the log files or locations that you specify, collects log events, and forwards them to your Vizion.ai elasticsearch instance.

## Installation:

### Windows:

1) As administrator, enter the following command in Powershell or download the zip file [here](https://github.com/themarcusaurelius/Filebeat/archive/master.zip).

```
Start-BitsTransfer -Source 'https://github.com/themarcusaurelius/Filebeat/archive/master.zip' -Destination 'C:\Users\Administrator\Downloads\filebeat.zip'
```

2) Unzip the package and extract the contents to the `C:/` drive.

3) Back in Powershell, CD into the extracted folder and run the following script:

```
.\installFilebeat.ps1
```

4) When prompted, enter your credentials below and click ```OK```.

```css
Kibana URL: _PLACEHOLDER_KIBANA_URL_
Username: _PLACEHOLDER_USERNAME_
Password: _PLACEHOLDER_PASSWORD_
Elasticsearch API Endpoint: _PLACEHOLDER_API_ENDPOINT_
```

5) Choose the path to the folder that has the data you would like to monitor and click ```OK```.

This will install and run filebeat.

**Data should now be shipping to your Vizion Elastic app. Check the ```Discover``` tab in Kibana for the incoming logs**

<i>If you would like to parse the logs in order to create visuals in Kibana, you will need to build an ingest pipeline or use one of the pre-built modules available for that certain log type.</i>

<hr>





# Logstash pipeline configuration files

List of Logstash pipeline configuration files, used for Stormshield product logs:
  * 11-filter-standard.conf Standard filter that performs some pre-tasks
  * 12-filter-sdmc.conf [Data For Cloud Mobility](https://www.stormshield.com/products/cloud-and-mobility/)
  * 13-filter-sds.conf [Data Enterprise](https://www.stormshield.com/products/enterprise)
  * 14-filter-ses.conf [Stormshield Endpoint Security](https://www.stormshield.com/products/stormshield-endpoint-security/)
  * 15-filter-sns.conf [Network Security](https://www.stormshield.com/products-services/products/network-security/)

## Installation instructions
  - Copy `01-input-syslog.conf` file in your _Logstash_ configuration path.
    - Update the **port** on which _Logstash_ is listening for trafic, if needed.
  - Copy `11-filter-standard.conf` and any _.conf_ files you want in your _Logstash_ configuration path
  - Copy `21-output-elasticsearch.conf` file in your _Logstash_ configuration path.
    - Replace **elasticsearch** host by your Elasticsearch instance hostname (eventually, update port number. Default _9200_), if needed.

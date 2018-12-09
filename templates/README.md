# Elasticsearch templates

List of Elasticsearch templates, used for Stormshield product logs:
  * sns.template.json [Network Security](https://www.stormshield.com/products-services/products/network-security/)
  * sdmc.template.json [Data For Cloud Mobility](https://www.stormshield.com/products/cloud-and-mobility/)
  * sds.template.json [Data Enterprise](https://www.stormshield.com/products/enterprise)
  * ses.template.json [Stormshield Endpoint Security](https://www.stormshield.com/products/stormshield-endpoint-security/)

## Installation instructions

  - For [Network Security](https://www.stormshield.com/products-services/products/network-security/) logs:
  ```bash
curl -XPUT http://<your-elasticsearch-server>:9200/_template/snslog -H 'Content-Type: application/json' -d @sns.template.json
```
  - For [Data For Cloud Mobility](https://www.stormshield.com/products/cloud-and-mobility/) logs:
  ```bash
curl -XPUT http://<your-elasticsearch-server>:9200/_template/sdmclog -H 'Content-Type: application/json' -d @sdmc.template.json
```
  - For [Data Enterprise](https://www.stormshield.com/products/enterprise) logs:
  ```bash
  curl -XPUT http://<your-elasticsearch-server>:9200/_template/sdslog -H 'Content-Type: application/json' -d @sds.template.json
```
  - For [Stormshield Endpoint Security](https://www.stormshield.com/products/stormshield-endpoint-security/) logs:
```bash
curl -XPUT http://<your-elasticsearch-server>:9200/_template/seslog -H 'Content-Type: application/json' -d @ses.template.json
```

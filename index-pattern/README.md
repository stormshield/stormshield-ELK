# Kibana index-pattern

List of Kibana index-pattern, used for Stormshield product logs:
  * stormshield-sns-fields-format.json [Network Security](https://www.stormshield.com/products-services/products/network-security/)
  * stormshield-sdmc-fields-format.json [Data For Cloud Mobility](https://www.stormshield.com/products/cloud-and-mobility/)
  * stormshield-sds-fields-format.json [Data Enterprise](https://www.stormshield.com/products/enterprise)
  * stormshield-ses-fields-format.json [Stormshield Endpoint Security](https://www.stormshield.com/products/stormshield-endpoint-security/)

## Installation instructions

  - For [Network Security](https://www.stormshield.com/products-services/products/network-security/) logs:
  ```bash
  curl -XPOST -D- 'http://localhost:5601/api/saved_objects/index-pattern' \
   -H 'Content-Type: application/json' \
   -H 'kbn-version: 5.6.7' \
   -H 'Content-Type: application/json' -d @stormshield-sns-fields-format.json
  ```
  - For [Data For Cloud Mobility](https://www.stormshield.com/products/cloud-and-mobility/) logs:
  ```bash
  curl -XPOST -D- 'http://localhost:5601/api/saved_objects/index-pattern' \
   -H 'Content-Type: application/json' \
   -H 'kbn-version: 5.6.7' \
   -H 'Content-Type: application/json' -d @stormshield-sdmc-fields-format.json
  ```
  - For [Data Enterprise](https://www.stormshield.com/products/enterprise) logs:
  ```bash
  curl -XPOST -D- 'http://localhost:5601/api/saved_objects/index-pattern' \
   -H 'Content-Type: application/json' \
   -H 'kbn-version: 5.6.7' \
   -H 'Content-Type: application/json' -d @stormshield-sds-fields-format.json
  ```
  - For [Stormshield Endpoint Security](https://www.stormshield.com/products/stormshield-endpoint-security/) logs:
  ```bash
  curl -XPOST -D- 'http://localhost:5601/api/saved_objects/index-pattern' \
   -H 'Content-Type: application/json' \
   -H 'kbn-version: 5.6.7' \
   -H 'Content-Type: application/json' -d @stormshield-ses-fields-format.json
  ```
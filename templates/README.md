# Elasticsearch templates

List of Elasticsearch templates, used for Stormshield product logs:

* sns-*.template.json [Network Security](https://www.stormshield.com/products-services/products/network-security/)
* sdmc-*.template.json [Data For Cloud Mobility](https://www.stormshield.com/products/cloud-and-mobility/)
* sds.template.json [Data Enterprise](https://www.stormshield.com/products/enterprise)
* ses-*.template.json [Stormshield Endpoint Security](https://www.stormshield.com/products/stormshield-endpoint-security/)

## Installation instructions

* For [Network Security](https://www.stormshield.com/products-services/products/network-security/) logs:

```bash
find . -maxdepth 1 -name 'sns-*.template.json' -execdir bash -c 'file=${0#./}; curl --user elastic:changeme -XPUT http://<your-elasticsearch-server>:9200/_template/${file%.template.json}?include_type_name=true -H "Content-Type: application/json" -d @${file}' {} \;
```

* For [Data For Cloud Mobility](https://www.stormshield.com/products/cloud-and-mobility/) logs:

```bash
find . -maxdepth 1 -name 'sdmc-*.template.json' -execdir bash -c 'file=${0#./}; curl --user elastic:changeme -XPUT http://<your-elasticsearch-server>:9200/_template/${file%.template.json}?include_type_name=true -H "Content-Type: application/json" -d @${file}' {} \;
```

* For [Data Enterprise](https://www.stormshield.com/products/enterprise) logs:

```bash
  curl --user elastic:changeme -XPUT http://<your-elasticsearch-server>:9200/_template/sds?include_type_name=true -H 'Content-Type: application/json' -d @sds.template.json
```

* For [Stormshield Endpoint Security](https://www.stormshield.com/products/stormshield-endpoint-security/) logs:

```bash
find . -maxdepth 1 -name 'ses-*.template.json' -execdir bash -c 'file=${0#./}; curl --user elastic:changeme -XPUT http://<your-elasticsearch-server>:9200/_template/${file%.template.json}?include_type_name=true -H "Content-Type: application/json" -d @${file}' {} \;
```

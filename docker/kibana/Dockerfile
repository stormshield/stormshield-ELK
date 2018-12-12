ARG ELK_VERSION

# https://github.com/elastic/kibana-docker
FROM docker.elastic.co/kibana/kibana:${ELK_VERSION}

#RUN curl -XPOST -u kibana:changeme -D- 'http://localhost:5601/api/saved_objects/index-pattern' \
#   -H 'Content-Type: application/json' \
#   -H 'kbn-version: 5.6.7' \
#   -H 'Content-Type: application/json' -d @/usr/share/kibana/index-pattern/stormshield-sns-fields-format.json
#RUN curl -XPOST -u kibana:changeme -D- 'http://localhost:5601/api/saved_objects/index-pattern' \
#   -H 'Content-Type: application/json' \
#   -H 'kbn-version: 5.6.7' \
#   -H 'Content-Type: application/json' -d @/usr/share/kibana/index-pattern/stormshield-sdmc-fields-format.json
#RUN curl -XPOST -u kibana:changeme -D- 'http://localhost:5601/api/saved_objects/index-pattern' \
#   -H 'Content-Type: application/json' \
#   -H 'kbn-version: 5.6.7' \
#   -H 'Content-Type: application/json' -d @/usr/share/kibana/index-pattern/stormshield-sds-fields-format.json
#RUN curl -XPOST -u kibana:changeme -D- 'http://localhost:5601/api/saved_objects/index-pattern' \
#   -H 'Content-Type: application/json' \
#   -H 'kbn-version: 5.6.7' \
#   -H 'Content-Type: application/json' -d @/usr/share/kibana/index-pattern/stormshield-ses-fields-format.json

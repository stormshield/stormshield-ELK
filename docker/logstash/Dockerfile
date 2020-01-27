ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

RUN logstash-plugin install logstash-filter-SNS
RUN logstash-plugin install logstash-filter-search-engine
RUN logstash-plugin install logstash-filter-SDS
RUN logstash-plugin install logstash-filter-SES

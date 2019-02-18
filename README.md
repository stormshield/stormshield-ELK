# Stormshield Elastic Stack

This project hosts files and links to components used by [Stormshield Visibility Center](https://www.stormshield.com/products/visibility-center).

## Installation instructions
  * Make sure you have a fully functional Elastic stack running. If not, please refer to [Installing the Elastic Stack](https://www.elastic.co/guide/en/elastic-stack/5.6/installing-elastic-stack.html#installing-elastic-stack) instructions,
  * Install [Syslog-ng](./syslog-ng)
  * Install [Kibana index-pattern](./index-pattern),
  * Install [Elasticsearch templates](./templates),
  * Install [Logstash plugins](#plugins),
  * Update [Logstash pipeline](./pipeline) configuration,
  * Configure your Stormshield products to send logs to your _Syslog-ng_ instance
    * UDP **514** or
    * TCP **601**

### Docker
A ready to use Elastic Stack is also provided as a Docker container for testing
, [here](./docker).

## Logstash
### Plugins
  * [logstash-filter-SNS](https://github.com/stormshield/logstash-filter-SNS)
  * [logstash-filter-SDS](https://github.com/stormshield/logstash-filter-SDS)
  * [logstash-filter-SES](https://github.com/stormshield/logstash-filter-SES)
  * [logstash-filter-search-engine](https://github.com/stormshield/logstash-filter-search-engine)

### Pipeline configuration
  List of [pipeline](./pipeline) configurations.

## Elasticsearch templates
  List of [templates](./templates).

## Kibana index-pattern
  List of [index-patterns](./index-pattern).

## Supported version
  * Elasticsearch: *5.6.7*
  * Kibana: *5.6.7*
  * Logstash: *5.6.7*

## Legal Disclaimer
Open source projects are made available and contributed to under licenses that include terms that, for the protection of contributors, make clear that the projects are offered “as-is”, without warranty, and disclaiming liability for damages resulting from using the projects. This guide is no different. The open content license it is offered under includes such terms.

Running an open source project, like any human endeavor, involves uncertainty and trade-offs. We hope this guide helps, but it may include mistakes, and can’t address every situation. If you have any questions about your project, we encourage you to do your own research, seek out experts, and discuss with your community. If you have any legal questions, you should consult with your own legal counsel before moving forward. If you’re at a company, talk to its legal team.

## Credit
SVC team:
  * [Alban MARGUET](mailto:alban.marguet@stormshield.eu)
  * [Laurent LEMKE](mailto:laurent.lemke@stormshield.eu)
  * [Nabil BENDAFI](mailto:nabil.bendafi@stormshield.eu)
  * [Thomas ESCURE](mailto:thomas.escure@stormshield.eu)

## Contact
Labo SVC <[labo.svc@stormshield.eu](mailto:labo.svc@stormshield.eu)>

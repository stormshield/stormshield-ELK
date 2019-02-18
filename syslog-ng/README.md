# Syslog-ng configuration files

Stormshield products send logs using different RFC standards. This _Syslog-ng_ configuration file is used to address every cases, since [Logstash](https://www.elastic.co/guide/en/logstash/current/plugins-inputs-syslog.html) _syslog_ input plugin only supports [RFC3164](https://www.ietf.org/rfc/rfc3164.txt)

## Installation instructions
  - Copy `syslog-stormshield-configuration.conf` file in your _Syslog-ng_ configuration path ( Default: _/etc/syslog-ng/conf.d/_)

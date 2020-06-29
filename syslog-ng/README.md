# Syslog-ng configuration files

Stormshield products send logs using different RFC standards. This _Syslog-ng_ configuration file is used to address every cases, since [Logstash](https://www.elastic.co/guide/en/logstash/current/plugins-inputs-syslog.html) _syslog_ input plugin only supports [RFC3164](https://www.ietf.org/rfc/rfc3164.txt)

## Installation instructions

* Modify the first line of the file `syslog-stormshield-configuration.conf`: _@version: 3.27.1 with you own _Syslog-ng_ version if needed
* Copy `syslog-stormshield-configuration.conf` file in your _Syslog-ng_ configuration path ( Default: _/etc/syslog-ng/conf.d/_)

## Deploy syslog-ng with docker-compose
* Create a directory to host your docker-compose configuration file. Put inside the docker-compose.yml
* Inside the directory created before, create a directory named "config.d" and put the "syslog-stormshield-configuration.conf" inside. Don't forget to modify the file following instructions above.
* Start container with
  ```bash
  docker-compose up -d
  ```

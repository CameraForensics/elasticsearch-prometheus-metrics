# prometheus-metrics plugin for ElasticSearch [![Build Status](https://travis-ci.org/jsuchenia/elasticsearch-prometheus-metrics.svg?branch=master)](https://travis-ci.org/jsuchenia/elasticsearch-prometheus-metrics)

[Elasticsearch](https://www.elastic.co/products/elasticsearch) plugin to return internal status data in [Prometheus](https://prometheus.io) format for monitoring purposes. It can deliver basic information about cluster, indices and JVM status

## Features

Run of variety of Elasticsearch versions without any dependency - just pure asynchroneus java - so it's not blocking threads with sync calls.

After installation it will expose few HTTP endpoints:
* */_prometheus/jvm* - with details about JVM - most of metric aligned with [client_java](https://github.com/prometheus/client_java) code
* */_prometheus/indices* - details about Indices stats
* */_prometheus/cluster* - CLuster and indices status
* */_prometheus* - Overall status

To use it just add target URL to your prometheus: `http://elasticsearch.domain.com:9200/_prometheus`

## Supported versions
* 5.4.0
* 5.3.2
* 5.3.1
* 5.3.0

Generated .zip plugins are available at Releases section of this project

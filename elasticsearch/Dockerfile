FROM docker.elastic.co/elasticsearch/elasticsearch:7.2.1

COPY configs/elasticsearch.yml /usr/share/elasticsearch/config/elasticsearch.yml

HEALTHCHECK --interval=10s --timeout=50s --retries=5 CMD curl --silent --fail localhost:9200/_cluster/health || exit 1

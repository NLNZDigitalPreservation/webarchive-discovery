FROM solr:7

USER root

# Add a collection with webarchive-discovery nzwebarchive schema:
ADD solr7 /opt/solr/server/solr/webarchive
RUN chown -R solr /opt/solr/server/solr/webarchive

# Add webarchive-discovery nzwebarchive schema to tmp for populating volume mount:
ADD solr7 /tmp/solr/webarchive
RUN chown -R solr /tmp/solr/webarchive

USER solr


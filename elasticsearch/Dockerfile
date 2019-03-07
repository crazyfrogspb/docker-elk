ARG ELK_VERSION

# https://github.com/elastic/elasticsearch-docker
FROM docker.elastic.co/elasticsearch/elasticsearch-oss:${ELK_VERSION}

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
ADD staysense-cosine-sim-6.6.1.zip .
RUN elasticsearch-plugin install file:staysense-cosine-sim-6.6.1.zip

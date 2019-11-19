ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

# Add your logstash plugins setup here
RUN logstash-plugin install logstash-filter-json
RUN logstash-plugin install logstash-filter-prune
RUN logstash-plugin install logstash-filter-ruby
RUN logstash-plugin install logstash-filter-date
RUN logstash-plugin install logstash-input-http_poller

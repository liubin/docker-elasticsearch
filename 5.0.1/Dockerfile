FROM elasticsearch:5.0.1

COPY docker-entrypoint.sh /

RUN wget https://artifacts.elastic.co/downloads/kibana/kibana-5.0.1-linux-x86_64.tar.gz \
  && tar -xzf kibana-5.0.1-linux-x86_64.tar.gz -C /opt \
  && rm kibana-5.0.1-linux-x86_64.tar.gz

EXPOSE 5601

COPY kibana.yml /opt/kibana-5.0.1-linux-x86_64/config/
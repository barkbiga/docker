FROM kibana
RUN \
  apt-get update && \
  apt-get install -y \
    libfontconfig \
    libfreetype6 && \
  rm -rf /var/lib/apt/lists/* && \
  usr/share/kibana/bin/kibana-plugin install x-pack
RUN  chown -R kibana:kibana /usr/share/kibana/optimize/

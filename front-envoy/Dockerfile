FROM envoyproxy/envoy:v1.18-latest
RUN apt-get update && apt-get -q install -y \
    curl
COPY front-envoy.yaml /etc/envoy/front-envoy.yaml
RUN chmod go+r /etc/envoy/front-envoy.yaml
CMD /usr/local/bin/envoy -c /etc/envoy/front-envoy.yaml
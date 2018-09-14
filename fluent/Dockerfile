FROM fluent/fluentd:v0.12-debian

ENV FLUENTD_CONF fluentd.conf
ADD fluentd.conf /fluentd/etc

RUN ["gem", "install", "fluent-plugin-elasticsearch", "--no-rdoc", "--no-ri", "--version", "1.9.2"]

ENTRYPOINT ["fluentd"]
CMD ["-c", "/fluentd/etc/fluentd.conf"]
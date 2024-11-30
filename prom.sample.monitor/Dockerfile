# Use the official Prometheus image as the base
FROM prom/prometheus:latest

# Copy the Prometheus configuration file into the container
COPY prometheus-config.yml /etc/prometheus/prometheus.yml

# Expose the default Prometheus port
EXPOSE 9090

# Set the default entrypoint to Prometheus
ENTRYPOINT ["/bin/prometheus"]

# Use the default Prometheus command
CMD ["--config.file=/etc/prometheus/prometheus.yml"]

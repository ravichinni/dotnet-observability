# dotnet-observability
- Simple Docker solution to demonstrate Observability in .NET using OpenTelemetry, Prometheus, Grafana and Jaeger
- This is based on the article [Example: Use OpenTelemetry with Prometheus, Grafana, and Jaeger](https://learn.microsoft.com/en-us/dotnet/core/diagnostics/observability-prgrja-example#9-distributed-tracing-with-jaeger)

# Usage
- docker-compose up
- Observability.web at http://localhost:7000

![Web App](./docs/images/observability.web.png)
- Observability.web metrics at : http://localhost:7000/metrics

![Web App Metrics](./docs/images/observability.web.metrics.png)
- Prometheus collector at: http://localhost:9090/

![Prometheus Collector](./docs/images/observability.prometheus.png)
- Grafana at http://localhost:3000/
	- Register
   	
   	![Grafana connection](./docs/images/observability.grafana.connection.png)
	- Create a connection to Prometheus with url as http://host.docker.internal:9090

    	![Grafana metrics](./docs/images/observability.grafana.metrics.png)
- Jaeger at http://localhost:16686/
![Jaeger Traces](./docs/images/observability.jaeger.png)

# Backlog

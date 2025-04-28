
# Observability

This project demonstrates the core principles of **observability** — covering **metrics**, **logging**, and **tracing** — using popular open-source tools like **Prometheus**, **Grafana**, **Alertmanager**, **Elasticsearch**, **Fluentbit**, **Kibana**, and **Jaeger**.  
It also includes deployment of the **OpenTelemetry demo application** to showcase end-to-end instrumentation and telemetry collection.

## 📚 What This Project Covers

- **Metrics Collection & Alerting**
  - Prometheus setup for scraping application metrics.
  - Alertmanager integration for alerting based on Prometheus rules.
  - Grafana dashboards for visualizing collected metrics.

- **Centralized Logging**
  - EFK (Elasticsearch + Fluentbit + Kibana) stack setup.
  - Fluentbit configuration for log forwarding.
  - Kibana dashboards for log analysis and visualization.

- **Distributed Tracing**
  - Jaeger setup for capturing and visualizing traces.
  - Service instrumentation using OpenTelemetry SDKs.

- **Demo Application**
  - Deployment of OpenTelemetry’s demo microservices application.
  - Each service instrumented for metrics, logs, and traces.

## 🛠️ Tools & Technologies

- **Prometheus**
- **Alertmanager**
- **Grafana**
- **Elasticsearch**
- **Fluentbit**
- **Kibana**
- **Jaeger**

## 📖 Learning Outcomes

Through this project, I:
- Learned how to instrument applications for observability.
- Understood the flow of metrics, logs, and traces through various backend systems.
- Practiced setting up a full observability stack from scratch.
- Strengthened my skills in using OpenTelemetry, Prometheus, Grafana, Jaeger, and the EFK stack.

## 📎 References

- [Prometheus Documentation](https://prometheus.io/docs/introduction/overview/)
- [Grafana Documentation](https://grafana.com/docs/)
- [Elasticsearch Documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html)
- [Fluentbit Documentation](https://docs.fluentbit.io/manual)
- [Kibana Documentation](https://www.elastic.co/guide/en/kibana/current/index.html)
- [Jaeger Documentation](https://www.jaegertracing.io/docs/)
- [OpenTelemetry Documentation](https://opentelemetry.io/docs/)

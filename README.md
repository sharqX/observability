
# Observability Demo

This project demonstrates the core principles of **observability** — covering **metrics**, **logging**, and **tracing** — using popular open-source tools like **Prometheus**, **Grafana**, **Alertmanager**, **Elasticsearch**, **Fluentd**, **Kibana**, and **Jaeger**.  
It also includes deployment of the **OpenTelemetry demo application** to showcase end-to-end instrumentation and telemetry collection.

## 📚 What This Project Covers

- **Metrics Collection & Alerting**
  - Prometheus setup for scraping application metrics.
  - Alertmanager integration for alerting based on Prometheus rules.
  - Grafana dashboards for visualizing collected metrics.

- **Centralized Logging**
  - EFK (Elasticsearch + Fluentd + Kibana) stack setup.
  - Fluentd configuration for log forwarding.
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
- **Fluentd**
- **Kibana**
- **Jaeger**
- **OpenTelemetry Demo App**
- **Docker Compose** (or Kubernetes if applicable)

## 📂 Repository Structure

\`\`\`bash
observability/
├── docker-compose.yml         # Docker Compose setup for local deployment
├── prometheus/
│   └── prometheus.yml          # Prometheus scrape configuration
├── grafana/
│   └── dashboards/             # Sample Grafana dashboards
├── efk/
│   ├── fluentd.conf            # Fluentd configuration for log forwarding
│   └── elasticsearch.yml       # Elasticsearch configurations (if customized)
├── jaeger/
│   └── jaeger-config.yml       # Jaeger setup configuration
├── opentelemetry-demo/
│   └── manifests/              # OpenTelemetry demo app configurations
└── README.md                   # Project documentation
\`\`\`

## 🚀 How to Run

### Prerequisites

- Docker & Docker Compose installed.
- (Optional) kubectl and a Kubernetes cluster, if deploying on Kubernetes.

### Quick Start (Docker Compose)

\`\`\`bash
git clone https://github.com/sharqX/observability.git
cd observability
docker-compose up -d
\`\`\`

This will spin up Prometheus, Grafana, Elasticsearch, Fluentd, Kibana, Jaeger, and the OpenTelemetry Demo App.

### Access the UIs

- **Prometheus**: \`http://localhost:9090\`
- **Grafana**: \`http://localhost:3000\`
  - Default credentials: \`admin/admin\`
- **Kibana**: \`http://localhost:5601\`
- **Jaeger UI**: \`http://localhost:16686\`

## 📈 Dashboards and Visualizations

- Prebuilt Grafana dashboards available in the `grafana/dashboards` directory.
- Jaeger shows distributed traces for services in the demo application.
- Kibana lets you search and analyze logs collected via Fluentd.

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
- [Fluentd Documentation](https://docs.fluentd.org/)
- [Kibana Documentation](https://www.elastic.co/guide/en/kibana/current/index.html)
- [Jaeger Documentation](https://www.jaegertracing.io/docs/)
- [OpenTelemetry Documentation](https://opentelemetry.io/docs/)

# FOSSIEM: Free and Open Source Security Information and Event Management Stack

Welcome to FOSSIEM, the ultimate open-source SIEM stack designed for comprehensive security monitoring and incident response. FOSSIEM integrates critical components for robust log management, real-time event correlation, user behavior analytics, and customizable dashboards. This stack leverages entirely free and open-source tools to ensure accessibility and extensibility for diverse environments and use cases. Whether you're a security professional or an IT enthusiast, FOSSIEM provides the necessary tools to enhance your security posture and streamline incident response efforts.

## Components

1. **Fluentd**: Log collector and forwarder.
2. **Loki**: Log aggregation and querying.
3. **Apache Kafka**: Stream processing for log data.
4. **Wazuh**: Security monitoring and event correlation.
5. **Apache Metron**: Real-time monitoring and analytics.
6. **Grafana**: Visualization and dashboarding.

## Prerequisites

- Docker
- Docker Compose

## Deployment

1. **Clone the Repository**

   ```sh
   git clone https://github.com/billyjstevens/FOSSIEM.git
   cd FOSSIEM
Start the Stack

sh
Copy code
docker-compose up -d
Access the Services

Grafana: http://localhost:3000 (default user: admin, default password: admin)
Wazuh: http://localhost:5601 (default user: admin, default password: admin)
Configuration
Fluentd
Configuration: fluentd/fluent.conf
Dockerfile: fluentd/Dockerfile
Loki
Configuration: loki/loki-config.yaml
Dockerfile: loki/Dockerfile
Kafka
Configuration: kafka/kafka-config.yaml
Dockerfile: kafka/Dockerfile
Wazuh
Configuration: wazuh/wazuh-config.yaml
Dockerfile: wazuh/Dockerfile
Grafana
Configuration: grafana/grafana.ini
Dockerfile: grafana/Dockerfile
Metron
Configuration: metron/metron-config.yaml
Dockerfile: metron/Dockerfile
Extensibility
This stack is designed to be highly extensible. You can add additional tools or modify configurations to suit your specific needs.

Contributing
Contributions are welcome! Please open an issue or submit a pull request.

License
This project is licensed under the MIT License.

# 🛒 Microservices-Based eCommerce Application

<p align="center">
  A scalable eCommerce platform built using Spring Boot Microservices, Apache Kafka, Eureka, API Gateway, Config Server, Keycloak, Zipkin, Prometheus, Grafana, and Loki.
</p>

<p align="center">
  <img width="100%" alt="eCommerce Architecture" src="assets/ecom.png" />
</p>

<hr/>

<h2>🚀 Architecture Overview</h2>

<p>
This project follows a decoupled microservices architecture with independent services, centralized configuration, service discovery, event-driven communication, distributed tracing, monitoring, and security.
</p>

<h2>🧩 Microservices & Ports</h2>

<ul>
  <li>👤 <strong>User Service</strong> — <code>8082</code></li>
  <li>📦 <strong>Product Service</strong> — <code>8083</code></li>
  <li>🧾 <strong>Order Service</strong> — <code>8084</code></li>
  <li>🔔 <strong>Notification Service</strong> — Kafka consumer-based</li>
</ul>

<h2>🔗 Supporting Services</h2>

<ul>
  <li>📘 <strong>Config Server</strong> — <code>8888</code></li>
  <li>🛰️ <strong>Eureka Server</strong> — <code>8761</code></li>
  <li>🚪 <strong>API Gateway</strong> — Unified entry point and routing</li>
  <li>📡 <strong>Apache Kafka</strong> — Asynchronous event streaming</li>
  <li>🔐 <strong>Keycloak</strong> — Authentication and authorization</li>
  <li>🔍 <strong>Zipkin</strong> — Distributed tracing</li>
  <li>📊 <strong>Prometheus</strong> — Metrics collection</li>
  <li>📈 <strong>Grafana</strong> — Monitoring dashboards and visualization</li>
  <li>🪵 <strong>Grafana Loki</strong> — Centralized log aggregation</li>
</ul>

<hr/>

<h2>📸 Project Screenshots</h2>

<h3>1. Eureka Server — Architecture & Service Registry</h3>
<p>Service registration and discovery across the microservices.</p>
<img width="100%" alt="Eureka architecture and service registry" src="assets/ecom-eureka.png" />

<h3>3. Circuit Breaker</h3>
<p>Resilience and fault tolerance through circuit breaker patterns.</p>
<img width="100%" alt="Circuit breaker dashboard" src="assets/circuit-breaker.png" />

<h3>4. Grafana Monitoring Dashboard</h3>
<p>Application and infrastructure metrics visualized using Grafana.</p>
<img width="100%" alt="Grafana monitoring dashboard" src="screenshots/dashboard with grafana springboot.png" />

<h3>5. Zipkin Distributed Tracing</h3>
<p>End-to-end request tracing across multiple microservices.</p>
<img width="100%" alt="Zipkin distributed tracing" src="assets/zipkin with gateway.png" />

<h3>6. Distributed Tracing with Grafana and Zipkin</h3>
<p>Trace visualization and analysis through Grafana using Zipkin data.</p>
<img width="100%" alt="Grafana Zipkin distributed tracing" src="assets/distrubuted tracind with zipkin.png" />

<h3>7. Grafana Loki Dashboard</h3>
<p>Centralized application logs collected and queried using Loki.</p>
<img width="100%" alt="Grafana Loki logs dashboard" src="assets/grafana loki dashbord.png" />

<h3>8. Prometheus CPU Usage</h3>
<p>CPU utilization metrics collected by Prometheus and visualized in Grafana.</p>
<img width="100%" alt="Prometheus CPU usage graph" src="assets/promethus cpu usage graph.png" />

<h3>9. API Rate Limiting</h3>
<p>Rate limiting configured to control request traffic and protect services.</p>
<img width="100%" alt="API rate limiting" src="assets/rate limitting.png" />

<h3>10. Distributed Tracing with Zipkin</h3>
<p>Detailed request traces showing service interactions, latency, and execution flow.</p>
<img width="100%" alt="Zipkin distributed trace" src="screenshots/distributed-tracing-zipkin.png" />

<hr/>

<h2>🔐 Security — Keycloak Integration</h2>

<ul>
  <li>Centralized authentication and authorization</li>
  <li>JWT-based access token validation</li>
  <li>Role-based access control (ADMIN / USER)</li>
  <li>Microservices validate tokens issued by Keycloak</li>
  <li>Protected API endpoints</li>
</ul>

<hr/>

<h2>✨ Key Features</h2>

<ul>
  <li>Service registration and discovery with Eureka</li>
  <li>Centralized configuration with Spring Cloud Config</li>
  <li>API Gateway with load-balanced routing</li>
  <li>Asynchronous messaging with Apache Kafka</li>
  <li>Fault tolerance with circuit breakers</li>
  <li>Distributed tracing with Zipkin</li>
  <li>Metrics collection with Prometheus</li>
  <li>Monitoring dashboards with Grafana</li>
  <li>Centralized logging with Grafana Loki</li>
  <li>API rate limiting</li>
  <li>Secured endpoints using Keycloak</li>
</ul>

<hr/>

<h2>▶️ Running the Project</h2>

<ol>
  <li>Start Keycloak</li>
  <li>Start Config Server (<code>8888</code>)</li>
  <li>Start Eureka Server (<code>8761</code>)</li>
  <li>Start API Gateway</li>
  <li>Start User, Product, and Order services</li>
  <li>Start Kafka and Zookeeper</li>
  <li>Start Notification Service</li>
  <li>Start Zipkin, Prometheus, Grafana, and Loki</li>
</ol>

<hr/>

<h2>📦 Tech Stack</h2>

<ul>
  <li>Java & Spring Boot</li>
  <li>Spring Cloud — Eureka, Config Server, Gateway</li>
  <li>Resilience4j — Circuit Breaker</li>
  <li>Keycloak — Authentication and Authorization</li>
  <li>Apache Kafka — Event Streaming</li>
  <li>MySQL / PostgreSQL / MongoDB</li>
  <li>Zipkin — Distributed Tracing</li>
  <li>Prometheus — Metrics Collection</li>
  <li>Grafana — Monitoring and Visualization</li>
  <li>Grafana Loki — Log Aggregation</li>
  <li>Docker — Containerization</li>
</ul>

<hr/>

<h2>📂 Screenshot Directory Structure</h2>

<pre>
screenshots/
├── ecommerce-architecture.png
├── eureka-architecture.png
├── service-discovery.png
├── circuit-breaker.png
├── grafana-dashboard.png
├── zipkin-tracing.png
├── grafana-zipkin-tracing.png
├── grafana-loki-dashboard.png
├── prometheus-cpu-usage.png
├── rate-limiting.png
└── distributed-tracing-zipkin.png
</pre>

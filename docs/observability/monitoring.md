# 📊 Monitoring and Metrics

## 1. Metrics Standard
Each service must expose `/metrics` endpoint.

**Example Metrics:**
- `http_requests_total`
- `http_request_duration_seconds`
- `service_error_total`

## 2. Tools
- **Prometheus** for metrics collection
- **Grafana** for dashboards

## 3. Alerting
Alerts configured in Prometheus rules:

## 4. Dashboards
Each service must define a Grafana dashboard JSON under `/observability/dashboards/`.

## 5. Tracing
Use OpenTelemetry SDK → Jaeger or Tempo backend.
# 🪵 Logging Standard

## 1. Format
Structured JSON logs with:
- timestamp
- level
- service
- trace_id
- message

**Example:**
```json
{
  "timestamp": "2025-10-13T09:30:00Z",
  "level": "info",
  "service": "order-service",
  "trace_id": "a12b34c56",
  "message": "Order created successfully"
}
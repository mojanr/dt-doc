# 🧩 Service: <Service Name>

## 1. Overview
Short description of the service’s purpose and its role in the system.

**Example:**
Handles user authentication and registration flows.

---

## 2. Responsibilities
- Main business functions
- Domain events emitted and consumed
- Key integrations with other services

---

## 3. API & Contract
### 3.1 REST / gRPC Endpoints
| Method | Endpoint | Description |
|--------|-----------|-------------|
| POST | `/api/v1/login` | User login |
| GET | `/api/v1/users/{id}` | Get user info |

### 3.2 Event Messages
| Event | Producer | Consumer | Schema |
|--------|-----------|----------|--------|
| `user.created` | user-service | email-service | [Schema link]() |

---

## 4. Data & Storage
| Type | Technology | Description |
|------|-------------|-------------|
| Database | PostgreSQL | Stores user profile data |
| Cache | Redis | Session tokens and temporary data |

Include migration notes or DB schema diagrams if available.

---

## 5. Configuration
| Variable | Description | Example |
|-----------|-------------|----------|
| `JWT_SECRET` | Secret for token signing | `abc123` |
| `DB_URL` | PostgreSQL connection | `postgres://...` |

---

## 6. Dependencies
List any upstream or downstream dependencies.

**Example:**  
Consumes APIs from `auth-service` and publishes events to `notification-service`.

---

## 7. Observability
- Expose `/health` and `/ready` endpoints.  
- `/metrics` endpoint for Prometheus.  
- Include tracing instrumentation (OpenTelemetry).

---

## 8. Security
- Auth method: Keycloak JWT  
- Role policy: `RBAC: USER, ADMIN`  
- Sensitive fields masked in logs.

---

## 9. Testing
| Type | Tool | Coverage |
|------|------|-----------|
| Unit | Jest | 80% |
| Integration | Supertest | Required |
| Contract | Pact | Required |

---

## 10. Deployment
Describe deployment steps, Helm chart path, or CI/CD pipeline reference.

---

## 11. Runbook & Troubleshooting
Common errors, known issues, and how to recover them.

---

## 12. Owner
| Team | Contact | Slack Channel |
|------|----------|----------------|
| Backend | @john | `#user-service` |

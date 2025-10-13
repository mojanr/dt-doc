# 🌐 API Design Guidelines

## 1. General Rules
- RESTful endpoints with plural nouns.
- Version in the path: `/api/v1/resource`.
- Support pagination, filtering, sorting.

## 2. Naming Convention
| Type | Convention |
|------|-------------|
| Endpoint | `/users/{id}` |
| Resource | Lowercase with hyphens |
| Query Params | `snake_case` |

## 3. Error Format
```json
{
  "code": "USER_NOT_FOUND",
  "message": "User not found",
  "status": 404
}
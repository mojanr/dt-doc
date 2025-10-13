# 🔐 Authentication Standard

## 1. Authentication Provider
- Centralized via **Keycloak**
- Supports **OIDC** and **OAuth2** flows
- Tokens issued as **JWT**

## 2. Token Validation
- Each service verifies JWT signature
- Token includes: `sub`, `role`, `exp`, `aud`
- Use middleware to enforce authentication

## 3. Token Lifespan
| Token Type | Expiration | Refresh |
|-------------|-------------|----------|
| Access | 15 min | Yes |
| Refresh | 7 days | No |

## 4. Example Middleware
_Pseudocode:_
```ts
function authGuard(req, res, next) {
  const token = req.headers.authorization;
  if (!validateToken(token)) return res.status(401);
  next();
}

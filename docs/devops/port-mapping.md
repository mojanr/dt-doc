# Port Mapping

| Service | Port | Description |
|---------|------|--------|
| dt-database-mariadb | 1011 |
| dt-database-postgre | 1021 |
| dt-database-mongo | 1031 |
| dt-cache-redis | 1041 | Port 1021 until 2019 are used for caching |
| dt-cid-komodo | 1051 | Port 1031 until 1039 are used for CI/CD |
| dt-auth-keycloak | 1061 | Port 1041 until 2019 are used for auth keycloak |
| dt-auth-casdoor | 1071 | Port 1051 until 2029 are used for auth casdoor
| dt-app | 3000 | Port 3000 and above are used for frontend application |
| dt-monitoring-grafana | 4001 | Port 4001 and above are used for monitoring and logging |
| dt-gateway-api-tyk | 5011 | Port 5011 until 5019 are used for gateway api | 
| dt-gateway-kafka | 5021 | Port 5021 until 5029 are used for gateway kafka |
| dt-gateway-mqtt | 5031 | Port 5031 until 5039 are used for gateway mqtt |
| dt-gateway-websocket | 5041 | Port 5041 until 5049 are used for gateway websocket | 
| dt-storage-minio | 6011 | Port 6011 until 6012 are used for storage minio |
| dt-storage-nextcloud | 6021 | Port 6021 until 6029 are used for storage nextcloud |
| dt-documentation-outline | 7011 | Port 7011 until 7012 above are used for documentation |
| dt-service-xxx | 8000 | Port 8000 and above are used for microservices and not exposed |
| dt-tps-xxx | 9001 | Port 9001 and above are used for third party service |
# Port Mapping

| Service | Expose Port | Origin Port | Description | Status |
|---------|------|--------|--------|--------| 
| dt-database-mariadb | 1011 | 3306 |||
| dt-database-postgre | 1021 | 5432 |||
| dt-database-mongo | 1031 | 27017 |||
| dt-cache-redis | 1051 | 6379 | Port 1051 until 1059 are used for caching |
| dt-cid-komodo | 1061 | 9120 | Port 1061 until 1069 are used for CI/CD |
| dt-auth-keycloak | 2011, 2012, 2013 | 8080, 8443, 900 | Port 2011 until 2019 are used for auth keycloak |
| dt-auth-casdoor | 2021, 2022, 2023 | 8000, 80, 443| Port 2021 until 2029 are used for auth casdoor
| dt-monitoring-grafana | 2031 | 3000 | Port 2031 until 2039 are used for monitoring and logging |
| dt-monitoring-collector-host | not exposed | 9090 | Port 2041 until 2049 are used for monitoring and logging |
| dt-gateway-api-tyk | 3011 | - | Port 3011 until 3019 are used for gateway api | 
| dt-gateway-kafka | 3021 | - | Port 3021 until 3029 are used for gateway kafka |
| dt-gateway-mqtt | 3031 | - | Port 3031 until 3039 are used for gateway mqtt |
| dt-gateway-websocket | 3041 |-| Port 3041 until 3049 are used for gateway websocket | 
| dt-documentation-api | 3051 | 8080 | Port 3051 until 3059 are used for gateway websocket | 
| dt-documentation | 3061 | - | Port 3061 until 3069 are used for gateway websocket | 
| dt-storage-minio | 4011 |-| Port 4011 until 4012 are used for storage minio |
| dt-storage-nextcloud | 4021 |-| Port 4021 until 4029 are used for storage nextcloud |
| dt-documentation-outline | 5011 |-| Port 5011 until 7012 above are used for documentation |
| dt-nginx | 6011 | 81, 8080, 8443 | Port 6011 until 7012 above are used for documentation |
| dt-app | not exposed || Port 3000 and above are used for frontend application |
| dt-service-xxx | not exposed || Port 8000 and above are used for microservices and not exposed |
| dt-tps-xxx | 9001 |-| Port 9001 and above are used for third party service |
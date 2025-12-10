# 📊 Règles d’observabilité

## Logs

- Format JSON structuré
- Inclus : timestamp, niveau, service, request_id, user_id (si applicable)
- Niveau `INFO` en prod, pas de logs en `DEBUG` bruyants

## Métriques

- Exposer un endpoint `/metrics` ou équivalent
- Suivre au minimum :
  - QPS
  - Latence p95 / p99
  - Taux d’erreurs (4xx / 5xx)

## Traces

- Intégrer OpenTelemetry si possible
- Propager un `trace_id` de bout en bout

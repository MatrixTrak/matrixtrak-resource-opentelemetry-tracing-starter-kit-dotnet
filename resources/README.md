# OpenTelemetry tracing starter kit (.NET)

This kit provides a minimal checklist and attribute map for production debugging.

## Files

- otel-trace-starter-checklist.md
- otel-attribute-map.md
- sampling-defaults.md

## How to use

1. Instrument inbound requests and one to two critical dependencies.
2. Propagate trace context across services.
3. Log trace id on errors and slow requests.

# OpenTelemetry attribute map (minimum)

## Service level

- service.name
- deployment.environment
- service.version

## HTTP inbound

- http.method
- http.route
- http.status_code
- url.scheme

## Dependency spans

- net.peer.name
- net.peer.port
- db.system
- db.name
- db.statement (avoid full query if high cardinality)

## Error fields

- error
- exception.type
- exception.message

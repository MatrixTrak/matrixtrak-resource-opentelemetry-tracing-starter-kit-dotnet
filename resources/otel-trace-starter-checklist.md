# OpenTelemetry tracing starter checklist (.NET)

Use this checklist to ship minimum viable tracing for production debugging.

## Entry points

- Trace every inbound HTTP request.
- Ensure trace context is propagated to outgoing HTTP and SQL calls.
- Log trace id and span id on errors and slow requests.

## Dependencies

- Instrument one to two critical dependencies first.
- Capture dependency name, duration, and status.
- Validate the slowest dependency spans show up in the trace.

## Sampling

- Sample 100 percent of errors.
- Sample 10 percent of successful requests.
- Increase only after you validate the signal quality.

## Validation

- Pick one incident scenario and verify the trace explains the latency.
- Confirm logs and traces join on trace id.

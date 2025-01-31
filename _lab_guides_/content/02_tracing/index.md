## Extend out-of-the-box distributed tracing with OpenTelemetry

Dynatrace's OneAgent is able to profile and instrument most programing languages. In most modern day application architectures, micro-services can come in a variety of programing languages. In order to enable distributed tracing across these polygot applications, Dynatrace leverages OpenTelemetry to extend its distributed tracing capabilites.

For the hands-on exercises, we've assembled a demo application based on Java. While the Frontend API Server benefits from the deep monitoring capabilities of OneAgent, the injection of an Agent Module into the Backend Server is not possible.

This section covers custom and automatic instrumentation with OpenTelemetry (traces) for Java, in order to link the spans produced within the Frontend all the way to the Backend, and form a complete distributed trace for each request.

What you will learn
- How to create custom spans and link them to existing traces
- How to enrich spans with relevant details
- How to simplify efforts using auto-instrumentation
- How to propagate context between different processes
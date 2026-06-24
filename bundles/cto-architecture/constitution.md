# CTO Constitution - Principios de Arquitectura

## Guardrails Globales

- **Simplicity First**: Preferir soluciones simples y mantenibles antes que over-engineering.
- **Security by Design**: Toda feature debe pasar security review.
- **Observability First**: Todo servicio crítico debe tener logging, metrics y tracing.
- **Cost Awareness**: Considerar siempre el costo operativo (especialmente en cloud).
- **Tech Debt Management**: Registrar y priorizar tech debt explícitamente.
- **Agent-Friendly Architecture**: Diseñar sistemas que sean fáciles de implementar y verificar por agentes IA.

## Decision Framework

1. **Trade-off Analysis** siempre requerido (performance vs costo vs mantenibilidad).
2. Usar patrones probados (Event-Driven, CQRS, Microservices solo cuando justificado).
3. Preferir estándares abiertos y herramientas maduras.
4. Preparar para horizontal scaling desde el día 1 cuando sea Growth stage.
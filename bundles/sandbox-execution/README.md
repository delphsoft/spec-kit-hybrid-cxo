# Sandbox Execution Bundle

**Permite a los agentes ejecutar código de forma segura en entornos aislados (inspirado en E2B).**

Este bundle proporciona ejecución segura de código (Python, Node.js, etc.) usando sandboxes aislados.

## Comandos Principales

- `/sandbox.execute` — Ejecuta código en un sandbox seguro
- `/sandbox.create-environment` — Crea entornos preconfigurados
- `/sandbox.run-tests` — Ejecuta tests en sandbox
- `/sandbox.analyze-output` — Analiza resultados de ejecución

## Integraciones
- CTO Agent: Code execution y testing
- QA Agent: Automated testing
- DevOps Agent: Deployment simulations
- Observability: Logging de ejecuciones

## Seguridad
- Usa aislamiento tipo Firecracker / E2B-style
- Timeouts y resource limits
- Output sanitization
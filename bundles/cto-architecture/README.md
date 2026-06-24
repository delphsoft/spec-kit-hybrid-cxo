# CTO Architecture Bundle

**Rol**: Chief Technology Officer - Arquitectura y Estrategia Técnica

Este bundle está diseñado para trabajar en conjunto con el **Product Manager Agent-Driven** y optimizar la arquitectura en proyectos impulsados por agentes IA.

## Principales capacidades

- Evaluación y propuesta de arquitectura
- Gestión de Tech Debt
- Decisiones de escalabilidad y performance
- Security by Design
- Cost optimization (cloud, infra)
- Elección de tecnologías y patrones

## Comandos disponibles (a través de extension)

- `/cto.architecture-review`
- `/cto.tech-debt-assessment`
- `/cto.scalability-plan`
- `/cto.security-review`
- `/cto.tech-stack-recommendation`
- `/cto.constitution` (aplica guardrails técnicos)

## Cómo usar

1. Después de `/pm.feature-breakdown` → Ejecutar `/cto.architecture-review`
2. Usar en conjunto con Spec Agent y Dev Agent
3. Siempre considerar el Stage Adapter (MVP / Growth / Enterprise)

Este bundle trabaja especialmente bien con el Product Manager Bundle.
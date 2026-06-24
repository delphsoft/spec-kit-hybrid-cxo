# Product Manager Bundle for AI Agent-Driven Development

**Nombre**: `product-manager`  
**Rol**: Chief Product Officer / Product Manager especializado en desarrollo con Agentes IA

Este bundle está **orientado específicamente** al desarrollo impulsado por agentes de IA (Spec-Kit, Cursor, Claude, etc.). Ayuda a sectorizar el trabajo en sub-equipos de agentes especializados.

## Filosofía
- El PM actúa como **orquestador de agentes**.
- Sectoriza el producto en dominios especializados (UI/UX Agent, Feature Agent, Spec Agent, etc.).
- Enfocado en **Spec-Driven Development** + validación continua.

## Comandos Principales (Skills)

### Core PM
- `/pm.roadmap` — Genera y mantiene roadmaps adaptados a estadio
- `/pm.prioritization` — Frameworks (RICE, MoSCoW, Value vs Effort, etc.)
- `/pm.stakeholder-analysis`
- `/pm.metrics-framework` — OKRs, North Star Metrics, AARRR, etc.

### Agent-Oriented Skills (Nuevas)
- `/pm.agent-orchestration` — Define estructura de agentes y responsabilidades
- `/pm.spec-review` — Revisión profunda de especificaciones
- `/pm.feature-breakdown` — Desglosa features en tareas para agentes
- `/pm.simulation-run` — Ejecuta simulaciones de usuario/flujo/negocio
- `/pm.uiux-brief` — Genera briefs detallados para agente UI/UX
- `/pm.dev-handover` — Prepara handoff técnico para equipo de devs/agentes de código

## Sectorización de Agentes (Recommended Structure)

### 1. **Spec Agent**
   - Responsable de escribir y refinar especificaciones de alta calidad.
   - Usa templates avanzados con secciones de Legal, CFO, CTO, etc.

### 2. **UI/UX Agent**
   - Genera wireframes, user flows, prototipos, design systems.
   - Comandos: `/uiux.generate-flow`, `/uiux.design-review`

### 3. **Feature Agent**
   - Implementa features completas siguiendo specs.
   - Enfocado en user stories + acceptance criteria.

### 4. **Simulation & Validation Agent**
   - Ejecuta simulaciones (usuario, edge cases, performance, costos).
   - Valida contra OKRs y riesgos.

### 5. **Dev Agent (Implementation)**
   - Código, tests, arquitectura (colabora con CTO Bundle).

## Templates Mejorados

- `spec-with-agents.md` → Template completo que incluye orquestación de agentes
- Secciones agregadas:
  - **Agent Assignment**
  - **Simulation Plan**
  - **UI/UX Requirements**
  - **Validation Criteria**
  - **Success Metrics por Agente**

## Integración con otros Bundles
- Trabaja junto a **CTO** (arquitectura), **Legal**, **CFO** y **Marketing**.
- Usa **Stage Adapter** para ajustar intensidad según MVP / Growth / Enterprise.

## Ejemplo de uso
```bash
/pm.agent-orchestration --feature "onboarding"
/pm.spec-review onboarding.spec.md
/uiux.generate-flow onboarding
```

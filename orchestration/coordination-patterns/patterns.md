# Patrones Detallados de Coordinación Multi-Agente

## 1. Sequential Workflow (Lineal)

**Descripción**: Las tareas se ejecutan una después de la otra, con handoff claro.

**Cuándo usarlo**:
- Features con dependencias fuertes
- Flujos críticos (ej: definir spec → architecture review → implementación)

**Ventajas**: Simple, fácil trazabilidad, bajo riesgo de inconsistencias.

**Implementación en Spec-Kit**:
- Flujo nativo: `/specify` → `/plan` → `/tasks` → `/implement`
- Uso de `/pm.agent-orchestration` con `mode: sequential`

**Ejemplo**:
```json
{
  "agents": ["Spec", "CTO", "Dev"],
  "mode": "sequential",
  "handoff": "output_to_input"
}
```

## 2. Parallel Execution

**Descripción**: Múltiples agentes trabajan simultáneamente en subtareas independientes.

**Cuándo usarlo**:
- UI/UX + Backend
- Research + Technical Validation
- Marketing experiments + Financial modeling

**Ventajas**: Velocidad, mejor uso de agentes paralelos.

**Riesgos**: Necesita buen merge strategy al final.

**Implementación**:
- `agent-coordination.json` con `parallel: true`
- COO Agent monitorea convergencia.

## 3. Hierarchical Orchestration (Recomendado principal)

**Descripción**: Product Manager Agent actúa como Orchestrator, delega a especialistas y consolida resultados.

**Niveles**:
- Level 0: PM Orchestrator
- Level 1: C-Level Agents (CTO, CFO, Marketing, Legal, COO)
- Level 2: Specialized Agents (UIUX, Feature, Simulation, etc.)

**Ventajas**: Escalabilidad, consistencia estratégica.

## 4. Debate & Consensus

**Descripción**: Agentes con perspectivas diferentes debaten y llegan a consenso.

**Cuándo**: Decisiones de arquitectura, pricing, riesgos altos.

**Técnica**: Round-robin de argumentos + votación ponderada o síntesis por PM.

## 5. Human-in-the-Loop (HITL)

**Puntos clave**:
- Aprobación de specs
- Revisión financiera
- Decisiones legales
- Go/No-Go de features

## 6. Adaptive Orchestration

**Descripción**: El flujo se ajusta dinámicamente según resultados intermedios (ej: si simulation falla → más análisis).

**Potenciado por**: Stage Adapter + COO Agent.

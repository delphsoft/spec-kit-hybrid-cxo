# Spec-Kit Hybrid CXO Bundles

Colección de **Bundles** y **Extensions** para Spec-Kit que incorporan roles ejecutivos (C-Level) + Legal.

## Bundles Incluidos

**Knowledge Base** (mejorado para RAG):
- `knowledge/bundle-summaries.md` → Resúmenes claros para que los agentes tengan contexto rico.

### CXO + Legal + Operations

- `cfo-financial` → **Suite completa de análisis financiero** con **validación automática de datos**, Unit Economics, Break-Even, Payback, Monte Carlo + gráficos, Matriz ponderada y Sensitivity Analysis
- `cto-architecture` → Arquitectura y estrategia técnica
- `cfo-financial` → **Suite completa de análisis financiero**: Unit Economics, Break-Even, Payback, Monte Carlo Simulation + gráficos, Matriz ponderada y Sensitivity Analysis
- `marketing-growth` → Estrategia de marketing y growth (Reforge-inspired)
- `legal-compliance` → Legal, privacidad y cumplimiento regulatorio
- `coo-operations` → **Operaciones, automatización de procesos y eficiencia escalable**

### PM & Strategy
- `product-manager` → **Gestión de producto orientada a desarrollo con Agentes IA** (Spec Agent, UI/UX Agent, Feature Agent, etc.)
- `agile-pm` → Agile / Scrum Master
- `business-strategist` → Estrategia de negocio y frameworks

## Instalación

```bash
git clone https://github.com/TU_USUARIO/spec-kit-hybrid-cxo.git
cd spec-kit-hybrid-cxo

# Agregar bundles
specify bundle add ./bundles/legal-compliance
```

## Uso

Ejemplo:
```
/legal.risk-assessment
/legal.compliance-checklist --stage mvp
```

## Presets de Metodologías

- **Agile/Scrum** — Sprints, retros, daily, backlog grooming
- **Kanban + Flow** — Visual management y optimización de flujo
- **Hybrid Project Management** — Agile + Waterfall / PMBOK
- **OKR + Strategy Deployment** — Objetivos y alineación estratégica
- **Lean Startup / Jobs-to-be-Done** — Validación rápida y customer-centric
- **Product Strategy** — Roadmapping, Prioritization (RICE, MoSCoW, etc.)

## Extensions PM & Strategy

- `/pm.sprint-plan`
- `/pm.risk-assessment`
- `/strategy.wardley-map`
- `/pm.stakeholder-analysis`
- `/pm.retrospective`
- Integraciones con Jira, Linear, Notion, etc.

## Stage Adapter

Preset transversal que adapta automáticamente bundles y metodologías según el estadio:
- **Startup MVP**
- **Growth / Scale-up**
- **Enterprise / Corporate**

---

**Contribuciones bienvenidas**. Ideal para equipos que quieren un desarrollo más profesional y alineado con negocio.
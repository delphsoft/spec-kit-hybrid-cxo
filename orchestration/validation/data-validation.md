# Data Validation Framework for Multi-Agent Decisions

## Propósito
Asegurar integridad, consistencia y calidad de los datos usados en análisis financieros, matrices de decisión, simulaciones Monte Carlo y orquestación de agentes.

## Reglas Generales de Validación

### 1. Validación Básica (siempre aplicar)
- **Tipos de datos**: Número positivo, porcentaje entre 0-100, fechas válidas, etc.
- **Rangos razonables**: Ej. CAC > 0, Retención entre 0-100%, Payback > 0 meses.
- **Consistencia**: Total de pesos en matriz = 100%.
- **Completitud**: Campos obligatorios no vacíos.

### 2. Validación Avanzada por Herramienta

#### Para Matriz Ponderada
- Suma de pesos == 100% (±0.1 tolerancia)
- Puntajes entre 1-10
- Al menos 3 criterios

#### Para Monte Carlo
- Número de iteraciones ≥ 1000
- Distribuciones válidas (Normal, Triangular, etc.)
- Correlaciones entre -1 y 1
- Variables con sentido de negocio (no negativas donde corresponda)

#### Para Payback / Break-Even
- Cash flows consistentes (no saltos ilógicos)
- Inversión inicial > 0

## Template de Validación

```markdown
### Validación de Datos - [Análisis]

**Resultado**: ✅ Pasó / ❌ Falló

**Errores encontrados**:
- [Lista]

**Advertencias**:
- [Lista]

**Datos corregidos / Sugerencias**:
...
```

**Comando nuevo**: `/validation.run` o integrado en `/cfo.*` y `/pm.*`
# Repositorio de entrega — Proceso de validación de software

**Curso:** Testing y Validación de Software — Maestría en Arquitectura de Software, Universidad de La Sabana
**Autores:** Fredy Orlando Pulido Quintero · Myriam Andrea Martinez Fontecha
**Profesor:** César Augusto Vega Fernández
**Fecha:** Junio de 2026

---

## Estructura del repositorio

Este repositorio organiza los tres entregables solicitados, cada uno en su propia carpeta:

```
entrega_validacion_software/
├── README.md
├── 01_Reportes_Defectos/
│   └── Reporte_Defectos_Priorizados_y_Trazabilidad.docx
├── 02_Dashboard_Metricas/
│   └── Registro_Defectos_Ciclo_de_Vida.xlsx
└── 03_Informe_Tecnico/
    └── Informe_Tecnico_Sintesis_Validacion.docx
```

---

## 1. Reportes de defectos priorizados con su respectiva trazabilidad

**Carpeta:** `01_Reportes_Defectos/`
**Archivo:** `Reporte_Defectos_Priorizados_y_Trazabilidad.docx`

Contiene, para cada uno de los ocho defectos identificados durante el curso (5 técnicos de las Unidades 3-4 + 3 de rendimiento del proyecto final):

- Identificación, clasificación, seguimiento y validación, y cierre (ciclo de vida completo de 8 estados).
- **Priorización**: ranking P1 (crítico/inmediato), P2 (importante) y P3 (diferible), combinando severidad y prioridad.
- **Trazabilidad**: requisito/funcionalidad relacionada, caso de prueba, commit/Pull Request y documento (Wiki) relacionado, tanto por defecto como en una matriz consolidada.

## 2. Dashboard con métricas de calidad visualizadas y analizadas

**Carpeta:** `02_Dashboard_Metricas/`
**Archivo:** `Registro_Defectos_Ciclo_de_Vida.xlsx`

Libro de Excel con 5 hojas:

| Hoja | Contenido |
|------|-----------|
| `Registro_Defectos` | Matriz completa de los 8 defectos, con ranking de priorización y fórmulas de días de resolución. |
| `Ciclo_de_Vida` | Fecha de transición de cada defecto por los 8 estados del ciclo de vida. |
| `Dashboard` | Tablero de indicadores: severidad, estado, categoría, ranking, **cumplimiento de SLO de rendimiento**, **cobertura JaCoCo**, 3 gráficos dinámicos y un bloque de **análisis escrito**. |
| `Trazabilidad` | Matriz de trazabilidad consolidada (requisito → caso de prueba → commit/PR → documento). |
| `Glosario_Estados` | Definición de cada estado del ciclo de vida del defecto. |

## 3. Informe técnico de síntesis del proceso de validación

**Carpeta:** `03_Informe_Tecnico/`
**Archivo:** `Informe_Tecnico_Sintesis_Validacion.docx`

Informe independiente que sintetiza los hallazgos y conclusiones de **todo** el proceso de validación (no solo los defectos): metodología y herramientas por nivel de prueba (unitarias, integración, sistema, rendimiento), resultados consolidados (cobertura JaCoCo, resultados de los 6 escenarios k6, cumplimiento de SLO), hallazgos principales, conclusiones, recomendaciones y referencias a los otros dos entregables de este repositorio.

---

## Trazabilidad entre entregables

Los tres documentos están enlazados entre sí:
- El **Informe Técnico** (3) referencia al **Reporte de Defectos** (1) para el detalle de cada caso, y al **Dashboard** (2) para las métricas de calidad.
- El **Reporte de Defectos** (1) referencia al **Dashboard** (2) para las fórmulas de tiempo de resolución y los gráficos dinámicos.
- El **Dashboard** (2) contiene la misma matriz de trazabilidad que el **Reporte de Defectos** (1), en formato de hoja de cálculo.

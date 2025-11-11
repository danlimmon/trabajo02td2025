# TD2025 · Decisión Multicriterio (AHP · ELECTRE · PROMETHEE)

## Contexto del problema
El departamento debe **contratar un servicio de catering** para eventos con público diverso y tiempos ajustados.  
La decisión afecta a **satisfacción de asistentes**, **cumplimiento de SLA logísticos** y **presupuesto**.

## Objetivo
Elegir la **mejor alternativa** equilibrando **coste (PREC)**, **calidad percibida (QUAL)**, **variedad y seguridad alimentaria (DIET)** y **fiabilidad logística (LOG)**.

## Datos
- **Alternativas**: seis proveedores (A1…A6) con perfiles diferenciados (precio, calidad, dietas, puntualidad).
- **Subcriterios**  
  - **PREC (min)**: P1 Precio p/p, P2 Envío  
  - **QUAL (max)**: Q1 Sabor, Q2 Presentación, Q3 Frescura  
  - **DIET (max)**: D1 Variedad dietas, D2 Alérgenos, D3 Personalización  
  - **LOG**: L1 Puntualidad (max), L2 Tiempo respuesta (min), L3 Incidencias/100 (min)  
- Los datos se normalizan a **0–1** (mayor=mejor); los “min” se invierten.

## Enfoque metodológico
- **AHP**: jerarquía criterios→subcriterios; ranking por score compuesto y consistencia.  
- **ELECTRE I**: relación de sobreclasificación y **núcleo** (alternativas no dominadas).  
- **PROMETHEE II**: flujos **Φ⁺/Φ⁻/Φ** y ranking total; análisis de sensibilidad en **coste** y **pesos**.

## Conclusión
Hay **convergencia** en un top-3 (**A5, A4, A3**).  
- **A5** destaca si se prioriza **calidad y variedad de dietas**.  
- **A4** pasa a 1.º si la **logística** es crítica (puntualidad/incidencias).  
- **A3** es opción robusta cuando **dietas** pesan casi tanto como la calidad.


---
title: "Mapa Global: Inmunología Básica y Clínica"
fecha: 2025-12-03
tipo: MOC
tags:
  - inmunologia
  - global
  - moc
---

# 🧬 Mapa Global: Inmunología Básica y Clínica

> [!ABSTRACT] Visión Sinóptica
> Este curso explora la lógica defensiva del organismo, desde los mecanismos moleculares de reconocimiento hasta la orquestación de respuestas efectoras complejas y sus implicaciones patológicas.
> 
> **Estructura del Conocimiento**:
> 1.  **Vigilancia (Unidad I)**: Detección innata y preparación.
> 2.  **Decisión (Unidad II)**: Reconocimiento específico y procesamiento de información.
> 3.  **Acción (Unidad III)**: Ejecución de la respuesta y consecuencias (salud o enfermedad).

---

## 🗺️ Arquitectura del Sistema Inmune

```mermaid
graph TD
    %% Estilos "Nature-like"
    classDef input fill:#e1f5fe,stroke:#01579b,stroke-width:2px,color:#01579b;
    classDef unit1 fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#2e7d32;
    classDef unit2 fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#ef6c00;
    classDef unit3 fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#c2185b;
    classDef outcome fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#7b1fa2;

    Input([🦠 Entrada de Patógeno]):::input --> U1_Innata
    
    subgraph U1 [Unidad I: Bases y Vigilancia]
        direction TB
        U1_Innata[Inmunidad Innata\nBarreras, PAMPs, Fagocitos]:::unit1
        U1_Anatomia[Arquitectura Linfoide\nGanglios, Bazo, Timo]:::unit1
        U1_Innata --> U1_Anatomia
    end

    U1_Anatomia --> U2_Reconocimiento

    subgraph U2 [Unidad II: Reconocimiento y Procesamiento]
        direction TB
        U2_Reconocimiento[Reconocimiento Molecular\nMHC, TCR, BCR]:::unit2
        U2_Senal[Señalización y Sinapsis\nCoestimulación, Citocinas]:::unit2
        U2_Reconocimiento --> U2_Senal
    end

    U2_Senal --> U3_Efector

    subgraph U3 [Unidad III: Respuesta y Patología]
        direction TB
        U3_Efector[Mecanismos Efectores\nTh1/Th2/Th17, CTL, Anticuerpos]:::unit3
        U3_Regulacion[Regulación y Memoria\nTregs, Tolerancia]:::unit3
        U3_Efector --> U3_Regulacion
    end

    U3_Regulacion --> Outcome_Salud([✅ Eliminación / Salud]):::outcome
    U3_Regulacion -- Fallo --> Outcome_Enfermedad([⚠️ Patología\nAutoimun, Hipersens, Cáncer]):::outcome

    %% Enlaces a MOCs
    click U1 "Unidad I/00_Unidad_I_MOC.md" "Ir a Unidad I"
    click U2 "Unidad II/00_Unidad_II_MOC.md" "Ir a Unidad II"
    click U3 "Unidad III/00_Unidad_III_MOC.md" "Ir a Unidad III"
```

---

## 📂 Módulos de Aprendizaje

### [[Unidad I/00_Unidad_I_MOC|Unidad I: Bases de la Inmunidad]]
**Enfoque**: Fundamentos biológicos y químicos.
- **Temas Clave**:
    - [[03_Inmunidad_Innata|Inmunidad Innata y PAMPs]]
    - [[06_Inmunogenos_Antigenos|Antígenos e Inmunogenicidad]]
    - [[08_Organos_Sistema_Inmune|Anatomía del Sistema Inmune]]
    - [[09_Inmunoglobulinas|Estructura de Inmunoglobulinas]]

### [[Unidad II/00_Unidad_II_MOC|Unidad II: Reconocimiento de Antígenos]]
**Enfoque**: Mecanismos moleculares de especificidad.
- **Temas Clave**:
    - [[11_Sistema_Complemento|Sistema del Complemento]]
    - [[16_MHC_Complejo_Mayor_Histocompatibilidad|Complejo Principal de Histocompatibilidad (MHC)]]
    - [[19_Reconocimiento_TCR|Reconocimiento por TCR y Sinapsis]]
    - [[15_Citocinas|Red de Citocinas]]

### [[Unidad III/00_Unidad_III_MOC|Unidad III: Efectores y Patología]]
**Enfoque**: Integración sistémica y consecuencias clínicas.
- **Temas Clave**:
    - [[20_Respuesta_Celular|Respuesta Celular (Th1/CTL)]]
    - [[22_Respuesta_Humoral|Respuesta Humoral (B Cells)]]
    - [[25_Tolerancia_Autoinmunidad|Tolerancia y Autoinmunidad]]
    - [[29_Hipersensibilidad|Hipersensibilidades (I-IV)]]
    - [[27_Inmunidad_Tumoral|Inmunología del Cáncer]]

---

## 🧠 Conceptos Transversales (Hubs)

Estos conceptos conectan las tres unidades y son fundamentales para una comprensión holística:

- **[[Inflamacion]]**: Desde la respuesta innata aguda (UI) hasta la crónica y patológica (UIII).
- **[[Memoria_Inmunologica]]**: El objetivo final de la vacunación y la respuesta adaptativa.
- **[[Diagnostico_Inmunologico]]**: Aplicación práctica de la teoría (ELISA, Citometría, Aglutinación) a lo largo de todo el curso.

---
> [!TIP] Consejo de Estudio
> Utilice este mapa para orientarse. Si se siente perdido en los detalles moleculares de la Unidad II, regrese aquí para ver cómo encajan en la "Gran Imagen" de la defensa del huésped.

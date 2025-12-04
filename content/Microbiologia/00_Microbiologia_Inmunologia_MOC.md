---
title: "Mapa Global: Inmunología Básica y Clínica"
fecha: 2025-12-03
tipo: MOC
tags:
  - inmunologia
  - global
  - moc
  - nature_review
---

# 🧬 Mapa Global: La Lógica de la Defensa Inmunológica

> [!ABSTRACT] Abstract
> Este curso de **Inmunología Básica y Clínica** deconstruye la respuesta biológica frente a la no-mismidad (*non-self*). Desde la detección molecular de patrones conservados (PAMPs) hasta la orquestación de respuestas linfocitarias altamente específicas, analizamos cómo el sistema inmune mantiene la homeostasis.
>
> **Eje Central**: La transición crítica de la **Inmunidad Innata** (rápida, germinal) a la **Adaptativa** (lenta, somática), mediada por la presentación de antígenos, y cómo la desregulación de este proceso conduce a la patología.

---

## 🗺️ The Immunological Timeline: From Breach to Memory

Este diagrama integra las tres unidades del curso en un flujo temporal continuo.

```mermaid
graph TD
    %% --- ESTILOS (Nature-like Palette) ---
    classDef pathogen fill:#ffcdd2,stroke:#c62828,stroke-width:2px,color:#c62828;
    classDef innate fill:#e1f5fe,stroke:#0277bd,stroke-width:2px,color:#0277bd;
    classDef apc fill:#fff9c4,stroke:#fbc02d,stroke-width:2px,color:#f9a825;
    classDef adaptive fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#2e7d32;
    classDef effector fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#7b1fa2;
    classDef pathology fill:#263238,stroke:#000000,stroke-width:2px,color:#ffffff;

    %% --- FASE 1: INNATA (0-96h) [UNIDAD I] ---
    subgraph Phase1 [Fase 1: Reconocimiento Innato e Inflamación]
        direction TB
        Pathogen(["🦠 Infección / Daño"]):::pathogen
        Barriers["Barreras Epiteliales"]:::innate
        PAMPs["PAMPs / DAMPs"]:::pathogen
        PRRs["Receptores PRR<br/>(TLR, NLR, RLR)"]:::innate
        Inflammation["🔥 Inflamación Aguda<br/>(IL-1, IL-6, TNF-a)"]:::innate
        Phagocytes["Fagocitos<br/>(Neutrófilos, Macrófagos)"]:::innate
        
        Pathogen --> Barriers
        Barriers -- Brecha --> PAMPs
        PAMPs --> PRRs
        PRRs --> Inflammation
        Inflammation --> Phagocytes
    end

    %% --- PUENTE: PRESENTACIÓN (Unidad II) ---
    subgraph Phase2 [Fase 2: La Sinapsis Inmunológica]
        direction TB
        DC["Célula Dendrítica<br/>(APC Profesional)"]:::apc
        Migration["Migración a Ganglio"]:::apc
        MHC["Procesamiento y Carga<br/>(MHC-I / MHC-II)"]:::apc
        Synapse(("Sinapsis<br/>(TCR-MHC)")):::adaptive
        Signals["3 Señales:<br/>1. Reconocimiento<br/>2. Coestimulación<br/>3. Citocinas"]:::adaptive

        Phagocytes --> DC
        DC --> Migration
        Migration --> MHC
        MHC --> Synapse
        Synapse --> Signals
    end

    %% --- FASE 3: ADAPTATIVA (Unidad III) ---
    subgraph Phase3 [Fase 3: Expansión y Efectores]
        direction TB
        NaiveT["Linfocito T Naive"]:::adaptive
        ClonalExp["Expansión Clonal"]:::adaptive
        
        %% Ramas Efectoras
        Th1["Th1 / CTL<br/>(Celular)"]:::effector
        Th2["Th2 / B Cell<br/>(Humoral)"]:::effector
        Th17["Th17<br/>(Mucosas)"]:::effector
        
        Signals --> NaiveT
        NaiveT --> ClonalExp
        ClonalExp --> Th1
        ClonalExp --> Th2
        ClonalExp --> Th17
    end

    %% --- OUTCOMES ---
    subgraph Outcomes [Resultados Clínicos]
        Resolution(["✅ Resolución y Memoria"]):::adaptive
        Chronic(["⚠️ Inflamación Crónica"]):::pathology
        Autoimmunity(["⚠️ Autoinmunidad"]):::pathology
        
        Th1 --> Resolution
        Th2 --> Resolution
        Th17 --> Resolution
        
        Th1 -- Fallo Regulación --> Autoimmunity
        Th2 -- Hipersensibilidad --> Chronic
    end

    %% --- LINKS ---
    click Phase1 "Unidad I/00_Unidad_I_MOC.md"
    click Phase2 "Unidad II/00_Unidad_II_MOC.md"
    click Phase3 "Unidad III/00_Unidad_III_MOC.md"
    click MHC "Unidad II/16_MHC_Complejo_Mayor_Histocompatibilidad.md"
    click Synapse "Unidad II/19_Reconocimiento_TCR.md"
    click Inflammation "Unidad I/03_Inmunidad_Innata.md"
```

---

## 🔬 Desglose Curricular y Mecanismos Clave

### [[Unidad I/00_Unidad_I_MOC|Unidad I: La Vigilancia Molecular]]
> **"El sistema inmune no ve patógenos, ve patrones."**

Esta unidad establece los fundamentos de la biología celular inmunológica. Nos centramos en cómo el organismo distingue lo propio de lo extraño utilizando receptores codificados en la línea germinal (**PRRs**).

#### 🔍 Zoom-In: Señalización Innata (TLRs)
*Referencia: [[03_Inmunidad_Innata#Vías de Señalización Intracelular]]*

```mermaid
graph TD
    PAMP["PAMP"] --> TLR{TLR}
    TLR -->|Mayoría| MyD88["MyD88"]
    TLR -->|TLR3/4| TRIF["TRIF"]
    
    MyD88 --> NFkB["NF-κB"]
    NFkB --> Citocinas["TNF, IL-1, IL-6<br/>(Inflamación)"]
    
    TRIF --> IRF3["IRF3/7"]
    IRF3 --> IFN["Interferones Tipo I<br/>(Antiviral)"]
    
    style NFkB fill:#ff9,stroke:#333
    style IFN fill:#9ff,stroke:#333
```

---

### [[Unidad II/00_Unidad_II_MOC|Unidad II: La Decisión de Atacar]]
> **"Sin presentación no hay respuesta."**

Aquí diseccionamos el evento más sofisticado de la inmunología: la **Presentación de Antígenos**. Analizamos la genética del **MHC**, la restricción que impone, y la bioquímica de la **Sinapsis Inmunológica**.

#### 🔍 Zoom-In: La Cascada del TCR
*Referencia: [[19_Reconocimiento_TCR#2. Cascada de Señalización (Señal 1)]]*

```mermaid
graph TD
    TCR["TCR + MHC-p"] --> Lck["Lck activada"]
    Lck --> ITAMs["Fosforilación ITAMs"]
    ITAMs --> ZAP70["ZAP-70"]
    ZAP70 --> LAT["LAT (Hub)"]
    
    LAT --> NFAT["Vía Calcio -> NFAT"]
    LAT --> NFkB["Vía PKC -> NF-κB"]
    LAT --> AP1["Vía MAPK -> AP-1"]
    
    NFAT --> IL2["IL-2 (Proliferación)"]
    NFkB --> IL2
    AP1 --> IL2
```

---

### [[Unidad III/00_Unidad_III_MOC|Unidad III: Guerra y Paz (Patología)]]
> **"El poder de destruir conlleva el riesgo de autodestruirse."**

Integramos los mecanismos anteriores para entender la eliminación de patógenos y qué sucede cuando los mecanismos de control (**Tolerancia**) fallan.

#### 🔍 Zoom-In: Mecanismos Citotóxicos
*Referencia: [[20_Respuesta_Celular#2. Mecanismos de Citotoxicidad (CD8+ y NK)]]*

```mermaid
graph TD
    CTL["CTL Activado"] -->|Sinapsis| Diana["Célula Infectada"]
    
    subgraph Killing [Mecanismos de Muerte]
        Via1["Vía Granular"] --> Perf["Perforina -> Poros"]
        Via1 --> Granz["Granzimas -> Caspasas"]
        
        Via2["Vía FasL"] --> Fas["Fas (CD95)"]
        Fas --> Casp8["Caspasa-8"]
    end
    
    Diana --> Killing
    Killing --> Apoptosis["Apoptosis"]
    style Apoptosis fill:#f99
```

---

## 🔗 Nodos Conceptuales (Hubs Transversales)

Para navegar el curso como un experto, piense en estos conceptos no como temas aislados, sino como hilos conductores:

1.  **[[Inflamacion]]**: Es el contexto necesario para cualquier respuesta. Sin inflamación, hay tolerancia (o ignorancia).
2.  **[[Coestimulacion]]**: El sistema de seguridad de "dos llaves" para evitar la autoinmunidad.
3.  **[[Memoria_Inmunologica]]**: La base biológica de la vacunación y la diferencia fundamental entre un superviviente y un individuo naive.

---
> [!NOTE] Nota Técnica sobre Diagramas
> Los diagramas de este MOC utilizan sintaxis Mermaid.js compatible con Quartz. Se han simplificado las interacciones para asegurar la compatibilidad visual.

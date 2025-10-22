---
title: Estados Financieros LGS
tags:
  - estados-financieros
  - LGS
  - NIC-NIIF
  - PCGE
  - Art-221-224-LGS
  - SMV
  - SUNAT
aliases:
  - Estados Financieros
  - EE.FF.
  - Financial Statements
  - Balance y Resultados
---

# Estados Financieros LGS

## 🎯 Concepto

Informes estructurados sobre situación financiera, rendimiento y flujos de efectivo (Arts. 221-224 LGS).

**Marco Perú:**
- **Contable:** NIC/NIIF oficializadas por CNC
- **Legal:** LGS N° 26887
- **Tributario:** SUNAT, Ley IR
- **Supervisor:** SMV (SAA), SBS (bancos)
- **Codificación:** PCGE (Plan Contable General Empresarial)

**Conexiones:** [[junta-general-accionistas|Aprobación Junta]] • [[dividendos|Base dividendos]] • [[reserva-legal|Detracción reserva]] • [[auditoria-externa|Auditoría]] • [[memoria-anual|Memoria]]

## 📊 Los 5 Estados Financieros Obligatorios

Según **Art. 223 LGS**, los estados financieros que deben preparar las sociedades son:

### 1. Estado de Situación Financiera (Balance General)

**Definición:** Presenta la situación patrimonial de la empresa en un momento determinado (fotografía).

**Estructura según NIC 1:**
```
ACTIVO                          PASIVO
├─ Activo Corriente            ├─ Pasivo Corriente
│  ├─ Efectivo y equivalentes  │  ├─ Cuentas por pagar
│  ├─ Cuentas por cobrar       │  ├─ Deudas a corto plazo
│  └─ Inventarios              │  └─ Parte corriente deuda LP
└─ Activo No Corriente         └─ Pasivo No Corriente
   ├─ Propiedades              
   ├─ Intangibles              PATRIMONIO
   └─ Inversiones              ├─ Capital social
                               ├─ Reservas (legal, facultativas)
                               ├─ Resultados acumulados
                               └─ Resultado del ejercicio
```

**Relación con LGS:**
- **Art. 51-52:** Capital social debe estar reflejado en el patrimonio
- **Art. 229:** Reserva legal debe aparecer separadamente
- **Art. 83:** Acciones de inversión (si existen) en patrimonio

### 2. Estado de Resultados (Estado de Ganancias y Pérdidas)

**Definición:** Muestra el desempeño financiero de la empresa durante un período (película).

**Estructura según NIC 1:**
```
Ingresos de actividades ordinarias
(-) Costo de ventas
= UTILIDAD BRUTA

(-) Gastos de ventas
(-) Gastos de administración
= UTILIDAD OPERATIVA

(+/-) Ingresos/gastos financieros
(+/-) Otros ingresos/gastos
= UTILIDAD ANTES DE IMPUESTOS

(-) Impuesto a la renta (29.5% en Perú)
= UTILIDAD NETA DEL EJERCICIO
```

**Relación con LGS:**
- **Art. 229:** De la utilidad neta se deduce 10% para reserva legal
- **Art. 230-231:** Utilidades distribuibles para dividendos
- **Art. 40:** Utilidad neta determina dividendos

### 3. Estado de Cambios en el Patrimonio Neto

**Definición:** Muestra los movimientos en las cuentas patrimoniales durante el ejercicio.

**Movimientos típicos:**
```mermaid
graph LR
    A[Patrimonio Inicial] --> B[+ Aportes de capital]
    B --> C[+ Utilidad del ejercicio]
    C --> D[- Reserva legal]
    D --> E[- Dividendos pagados]
    E --> F[+/- Ajustes NIC 8]
    F --> G[Patrimonio Final]
```

**Relación con LGS:**
- **Art. 76-81:** Aumentos de capital
- **Art. 215-220:** Reducción de capital
- **Art. 229:** Aplicación de utilidades y constitución de reservas
- **Art. 230-231:** Distribución de dividendos

### 4. Estado de Flujos de Efectivo

**Definición:** Presenta las entradas y salidas de efectivo clasificadas por actividades.

**Estructura según NIC 7:**
```
FLUJOS DE ACTIVIDADES DE OPERACIÓN
+ Cobranzas a clientes
- Pagos a proveedores
- Pagos de personal
- Pagos de impuestos
= Flujo neto de operación

FLUJOS DE ACTIVIDADES DE INVERSIÓN
- Compra de activos fijos
+ Venta de activos fijos
= Flujo neto de inversión

FLUJOS DE ACTIVIDADES DE FINANCIAMIENTO
+ Aportes de accionistas
+ Préstamos recibidos
- Pago de préstamos
- Pago de dividendos
= Flujo neto de financiamiento

= AUMENTO/DISMINUCIÓN NETO DE EFECTIVO
```

**Relación con LGS:**
- **Art. 76:** Aportes en efectivo (flujo de financiamiento)
- **Art. 230-231:** Pago de dividendos (flujo de financiamiento)
- **Art. 215:** Devolución de aportes (flujo de financiamiento)

### 5. Notas a los Estados Financieros

**Definición:** Explicaciones y desagregaciones de las cifras presentadas en los estados financieros.

**Contenido mínimo según NIC 1:**
- Políticas contables aplicadas
- Juicios críticos y estimaciones
- Composición de saldos significativos
- Contingencias y compromisos
- Eventos posteriores al cierre

**Relación con LGS:**
- **Art. 223:** Las notas son parte integrante de los EE.FF.
- **Art. 176:** Deben revelar operaciones con partes relacionadas
- **Art. 223:** Deben incluir cuadros, notas y anexos

## 📅 Obligaciones Legales en Perú

### Plazos según LGS

| Obligación | Plazo | Base Legal |
|------------|-------|------------|
| **Preparación de EE.FF.** | Dentro de los 3 meses siguientes al cierre del ejercicio | Art. 221 LGS |
| **Aprobación por Junta** | Dentro de los 3 meses siguientes al cierre (reunión anual obligatoria) | Art. 114 LGS |
| **Dictamen del auditor** | Antes de la Junta (para SAA es obligatorio) | Art. 226 LGS |
| **Publicación (SAA)** | Después de aprobación, según reglamento SMV | Art. 224 LGS |

### Presentación a SUNAT

Según el **Reglamento de Libros Electrónicos (PLE):**

- **Libro de Inventarios y Balances:** Incluye Estado de Situación Financiera y Estado de Resultados
- **Plazo:** Dentro del mes siguiente al vencimiento del plazo para la Junta
- **Formato:** Electrónico a través del Sistema PLE-SUNAT

## 🔗 Integración Derecho-Contabilidad

### Tabla de Integración LGS-NIC/NIIF

| Cuenta del Balance | Regulación LGS | Norma Contable | Aplicación Práctica |
|-------------------|---------------|----------------|---------------------|
| **Capital Social** | Art. 51-52, 76-81 | NIC 32 | Emisión de acciones, aportes dinerarios y no dinerarios |
| **Reserva Legal** | Art. 229 | NIC 1 | 10% de utilidad neta hasta alcanzar 20% del capital |
| **Resultados Acumulados** | Art. 229-231 | NIC 1 | Utilidades no distribuidas de ejercicios anteriores |
| **Dividendos por Pagar** | Art. 230-231 | NIC 1 | Obligación de pagar 30% mínimo si hay utilidades distribuibles |
| **Acciones de Inversión** | Art. 83 | NIC 32 | Instrumento patrimonial sin derecho a voto |

## 🎯 Casos Prácticos

### Caso 1: Aplicación de Utilidades en una SA

**Situación:**
- Empresa SA "Comercial Lima S.A." cerró el ejercicio 2023 con utilidad neta de S/ 500,000
- Capital social: S/ 1,000,000
- Reserva legal acumulada: S/ 150,000

**Aplicación según LGS:**

```
Utilidad Neta 2023: S/ 500,000

1. Reserva Legal (Art. 229):
   10% x 500,000 = S/ 50,000
   Nueva reserva legal = 150,000 + 50,000 = S/ 200,000
   (Ya alcanzó el 20% del capital, por lo que esta sería la última detracción)

2. Utilidad Distribuible:
   500,000 - 50,000 = S/ 450,000

3. Dividendo Mínimo Obligatorio (Art. 231):
   Si hay utilidades distribuibles y un accionista lo solicita:
   30% x 450,000 = S/ 135,000 mínimo a distribuir

4. Junta decide distribuir:
   - Dividendos: S/ 300,000
   - Reserva facultativa: S/ 100,000
   - Utilidades retenidas: S/ 50,000
```

**Asiento Contable (según PCGE Perú):**
```
------- Por la detracción de reserva legal -------
59 RESULTADOS ACUMULADOS                50,000
   591 Utilidades no distribuidas
      58 RESERVAS                               50,000
         582 Legal

------- Por la declaración de dividendos -------
59 RESULTADOS ACUMULADOS               300,000
   591 Utilidades no distribuidas
      44 CUENTAS POR PAGAR DIVERSAS           300,000
         441 Dividendos por pagar
```

### Caso 2: Balance y Aumento de Capital

**Situación:**
La Junta General de "Inversiones Sur SAC" aprueba aumentar el capital de S/ 200,000 a S/ 300,000 mediante:
- Nuevos aportes en efectivo: S/ 50,000
- Capitalización de utilidades: S/ 50,000

**Impacto en el Balance:**

**ANTES del aumento:**
```
PATRIMONIO
Capital Social              200,000
Reserva Legal                20,000
Resultados Acumulados        80,000
Total Patrimonio           300,000
```

**DESPUÉS del aumento:**
```
PATRIMONIO
Capital Social              300,000  (+100,000)
Reserva Legal                20,000  (sin cambio)
Resultados Acumulados        30,000  (-50,000 por capitalización)
Total Patrimonio           350,000  (+50,000 por nuevo aporte)
```

**Cumplimiento Legal:**
- **Art. 76-77 LGS:** Acuerdo de Junta con mayoría calificada
- **Art. 80 LGS:** Derecho de preferencia de accionistas existentes
- **Art. 199 LGS:** Inscripción en SUNARP

## 💼 Responsabilidad de los Administradores

### Art. 221 LGS - Obligación de Preparar EE.FF.

**Responsables:**
- **Gerente General:** Firma los EE.FF.
- **Directorio:** Revisa y presenta a la Junta
- **Contador:** Prepara técnicamente los EE.FF.

**Consecuencias del incumplimiento:**
1. **Responsabilidad Civil:** Art. 177-184 LGS (daños a la sociedad o terceros)
2. **Infracciones Tributarias:** Multas SUNAT por no llevar libros contables
3. **Sanciones SMV:** Para SAA, multas por no presentar información

### Art. 223 LGS - Formulación y Contenido

> "Los estados financieros se preparan y presentan de conformidad con las disposiciones legales sobre la materia y con principios de contabilidad generalmente aceptados en el país."

**Interpretación del Comité de Expertos:**
- **"Principios generalmente aceptados"** en Perú = **NIC/NIIF** adoptadas por el CNC
- Obligación de aplicar todas las normas vigentes
- Las notas son obligatorias y parte integral de los EE.FF.

## 📚 Conexiones

### Dentro del Curso
- [[memoria-anual]] - Complementa los EE.FF. con información cualitativa
- [[auditoria-externa]] - Dictamen sobre razonabilidad de los EE.FF.
- [[reserva-legal]] - Se calcula y registra desde el Estado de Resultados
- [[dividendos]] - Se determinan a partir de las utilidades en EE.FF.
- [[sociedad-anonima-concepto]] - Órganos responsables de EE.FF.
- [[04-indice-unidad-4-informacion-financiera]] - Índice de esta unidad

### Con Otras Materias
- **Contabilidad Financiera:** Preparación técnica de EE.FF.
- **Auditoría:** Examen de razonabilidad de EE.FF.
- **Finanzas:** Análisis financiero (ratios, indicadores)
- **Tributación:** Determinación del IR a partir del Estado de Resultados

## 🔑 Referencias Normativas

### Marco Legal Peruano
- **Ley N° 26887 - LGS:**
  - Art. 221: Obligación de preparar estados financieros
  - Art. 222: Responsabilidad del directorio y gerencia
  - Art. 223: Formulación y contenido de los estados financieros
  - Art. 224: Publicación (para SAA)

### Marco Contable
- **NIC 1:** Presentación de Estados Financieros
- **NIC 7:** Estado de Flujos de Efectivo
- **NIC 8:** Políticas Contables, Cambios en Estimaciones y Errores
- **NIIF 15:** Ingresos de Actividades Ordinarias con Clientes
- **Resolución CNC:** Oficialización de NIC/NIIF en Perú

### Marco Tributario
- **TUO Ley del IR (D.S. 179-2004-EF):** Base para determinar impuesto
- **Resolución SUNAT N° 286-2009:** Reglamento PLE (Libros Electrónicos)

## ❓ Preguntas de Autoevaluación

1. ¿Cuáles son los 5 estados financieros obligatorios según la LGS?
2. ¿En qué plazo deben prepararse los EE.FF. después del cierre del ejercicio?
3. ¿Qué porcentaje de la utilidad neta se destina a reserva legal y hasta qué límite?
4. ¿Cómo se relaciona el Estado de Resultados con la distribución de dividendos?
5. ¿Qué información debe revelarse en las Notas a los EE.FF.?
6. ¿Qué diferencia hay entre el Balance General y el Estado de Resultados?
7. ¿Cuál es la responsabilidad del Gerente y del Directorio respecto a los EE.FF.?

---

**Elaborado por el Comité de Expertos:** Pedagogos, Documentadores, Psicólogos del Conocimiento, Expertos en Obsidian, Abogados y Contadores especializados en marco normativo peruano.

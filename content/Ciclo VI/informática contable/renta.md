---
dg-publish: true
title: Cálculo de Impuesto a la Renta 2024
draft: true
---

# 💼 Cálculo de Impuesto a la Renta — Persona Natural (Perú 2024)

> **Instrucciones:**  
> Edita los valores de **UIT** y **INGRESO_ANUAL** según corresponda.  
> El cálculo se actualiza automáticamente gracias a `DataviewJS`.

---

**Parámetros:**

- UIT:: 5150  
- INGRESO_ANUAL:: 180000  

---

```dataviewjs
// === Cálculo de Impuesto a la Renta 2024 ===
// Tomamos los valores declarados arriba en la nota
let UIT = dv.current().UIT ?? 5150;
let INGRESO_ANUAL = dv.current().INGRESO_ANUAL ?? 0;

// Declaramos variable del impuesto
let impuesto = 0;

// Tramos progresivos
if (INGRESO_ANUAL <= UIT * 15) {
	impuesto = INGRESO_ANUAL * 0.08;
} else if (INGRESO_ANUAL <= UIT * 35) {
	impuesto = UIT * 15 * 0.08 + (INGRESO_ANUAL - UIT * 15) * 0.14;
} else if (INGRESO_ANUAL <= UIT * 45) {
	impuesto = UIT * 15 * 0.08 + UIT * 20 * 0.14 + (INGRESO_ANUAL - UIT * 35) * 0.17;
} else if (INGRESO_ANUAL <= UIT * 60) {
	impuesto = UIT * 15 * 0.08 + UIT * 20 * 0.14 + UIT * 10 * 0.17 + (INGRESO_ANUAL - UIT * 45) * 0.20;
} else {
	impuesto = UIT * 15 * 0.08 + UIT * 20 * 0.14 + UIT * 10 * 0.17 + UIT * 15 * 0.20 + (INGRESO_ANUAL - UIT * 60) * 0.30;
}

// Mostramos resultado
dv.paragraph(`💰 **Impuesto calculado:** S/ ${impuesto.toFixed(2)}`);

// Información adicional
let tasaEf = (impuesto / INGRESO_ANUAL) * 100;
dv.paragraph(`📊 **Tasa efectiva:** ${tasaEf.toFixed(2)}%`);

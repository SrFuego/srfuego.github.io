---
dg-publish: true
---

# Banco de preguntas — INFORMÁTICA CONTABLE

Este banco está organizado por temas/conceptos derivados del sílabo y los balotarios existentes (Práctica Calificada N°1 y Examen Parcial). Para cada tema se incluyen al menos 7 preguntas — mezcla de conceptuales, aplicadas y casos prácticos — pensadas para evaluaciones, prácticas de laboratorio y exámenes.

---

## Tema: Hardware y Software (Ofimática y herramientas)

1. Defina con sus propias palabras qué es hardware y qué es software. Dé dos ejemplos de cada uno indispensables para el trabajo contable.
2. Explique la diferencia entre software de sistema y software de aplicación, dando un ejemplo contable de cada uno.
3. Mencione tres componentes de hardware internos de una computadora y describa cómo afectan el procesamiento de grandes volúmenes de datos contables.
4. ¿Qué periféricos consideraría imprescindibles para la emisión de comprobantes electrónicos y por qué?
5. Explique cómo una hoja de cálculo automatiza el cálculo de impuestos y da un ejemplo concreto (fórmula o función a usar).
6. Describa el procedimiento para crear una plantilla de Excel segura para registros contables (validaciones, protección de hoja, backups).
7. Caso práctico: Una empresa necesita imprimir y archivar comprobantes electrónicos impresos por contingencia. Describa el flujo de hardware y software necesario y los controles que implementaría.

---

## Tema: Sistemas informáticos (mono/multiusuario) y Gobierno Digital

1. Explique la diferencia entre un sistema monousuario y uno multiusuario y dé un ejemplo de cada en el contexto contable.
2. ¿Qué es el Sistema Nacional de Transformación Digital y por qué es importante para la modernización de procesos tributarios en el Perú?
3. Mencione tres ventajas y tres riesgos de migrar los procesos contables a sistemas multiusuario en la nube.
4. Explique qué controles de acceso y permisos son necesarios en un sistema contable multiusuario para proteger la integridad de los libros.
5. Desde la perspectiva del Gobierno Digital, ¿qué beneficios trae el uso del PDT y la Planilla Electrónica para la administración tributaria y las empresas?
6. Discuta cómo la interoperabilidad entre sistemas (ERP, sistemas bancarios, SUNAT) facilita la gestión tributaria. Dé un ejemplo concreto.
7. Caso práctico: Diseñe una política mínima de seguridad y continuidad para una empresa que empieza a usar SEE y PLE (incluya backups, roles y permisos, y plan de contingencia).

---

## Tema: Inteligencia Artificial aplicada a la contabilidad

1. Defina Inteligencia Artificial y mencione dos aplicaciones que mejoren procesos contables (por ejemplo, conciliaciones automáticas y detección de fraude).
2. Explique cómo un modelo de IA podría ayudar a detectar facturas duplicadas o incoherentes antes de subir al PLE.
3. ¿Qué datos y características serían útiles para entrenar un modelo de IA que prediga discrepancias entre ventas reportadas y pagos bancarios?
4. Discuta riesgos y consideraciones éticas al aplicar IA en procesos contables (privacidad, sesgo, trazabilidad).
5. Caso práctico: Diseñe un flujo simple (ETL + modelo) que automatice la conciliación bancaria y detalle métricas para evaluar su rendimiento.
6. Explique la diferencia entre automatización por reglas (scripts/macros) y automatización con IA. ¿En qué casos conviene usar cada una?
7. Proponga tres pruebas (tests) que se deben realizar antes de poner en producción un sistema de IA para auditoría contable.

---

## Tema: Programa de Declaración Telemática (PDT) y Declaraciones

1. ¿Qué es el PDT y cuál es su objetivo en el sistema tributario peruano?
2. Diferencie Declaración Determinativa y Declaración Informativa con un ejemplo de cada administrado vía PDT o plataformas SUNAT.
3. Enumere y describa los pasos básicos para presentar una declaración mensual de IGV-Renta usando PDT 621.
4. ¿Qué tipos de errores son comunes al llenar el PDT y cómo evitarlos (validaciones previas en Excel)?
5. Compare PDT 621 con Declara Fácil 621: público objetivo, limitaciones y ventajas.
6. Caso práctico: Explique qué haría si al intentar enviar el PDT obtiene un error de validación por inconsistencias en la SUNAT (pasos para detectar y corregir).
7. ¿Qué documentos o respaldos debería conservar un contador después de presentar una declaración telemática y por cuánto tiempo, según buenas prácticas?

---

## Tema: Bases de Datos y gestión de datos (import/export)

1. Defina base de datos y explique por qué es fundamental para sistemas de información contable.
2. ¿Qué es una relación en una base de datos relacional? Dé un ejemplo usando entidades: clientes, facturas, productos.
3. Explique la importancia de las funciones de importación y exportación en un software contable. Dé un ejemplo práctico.
4. Describa un flujo ETL básico para preparar datos de ventas mensuales para el PLE.
5. Caso práctico: Tiene un archivo CSV con caracteres especiales y formatos de fecha inconsistentes. Describa los pasos para limpiarlo y convertirlo al formato requerido por el PLE.
6. ¿Qué medidas de integridad (constraints) recomendaría para una base de datos contable para evitar duplicados y errores de suma?
7. Explique cómo un análisis de datos (por ejemplo, análisis de tendencias de ventas) extraído de la base contable puede apoyar decisiones gerenciales.

---

## Tema: Sistema de Emisión Electrónica (SEE) y comprobantes electrónicos

1. ¿Qué es el SEE según SUNAT y cuál es su objetivo principal?
2. Compare la emisión manual/impresa con la electrónica: mencione al menos 3 ventajas y 2 desventajas de la electrónica.
3. Describa al menos tres tipos de SEE que ofrece SUNAT y para qué cada uno es recomendable.
4. Explique el proceso de firma electrónica en la emisión de un comprobante electrónico y su importancia legal.
5. Caso práctico: Un cliente reporta facturas que no aparecen en su cuenta de operaciones. Explique cómo verificar si fueron emitidas correctamente y enviadas a SUNAT.
6. ¿Qué controles implementaría para asegurar que todos los comprobantes emitidos sean registrados en los libros electrónicos?
7. Explique el concepto de contingencia en emisión electrónica y describa procedimientos para emitir comprobantes durante una caída del servicio.

---

## Tema: Libros Electrónicos — PLE y SIRE (CUO, formatos, validaciones)

1. Explique qué es el PLE y qué tipos de libros se presentan mediante este programa.
2. ¿Qué es el CUO y por qué es importante dentro de los Libros Electrónicos?
3. Compare PLE y SIRE: funcionalidades y ventajas de cada uno.
4. Describa los principales errores de validación en las cargas del PLE y cómo corregirlos.
5. Caso práctico: Le devuelven un archivo PLE por error de CUO duplicado. Explique causas comunes y las acciones correctivas.
6. Liste al menos 10 campos obligatorios que deben incluirse en un registro de ventas para el PLE.
7. Explique cómo realizar una conciliación entre el Libro de Ventas electrónico (PLE) y los reportes bancarios para detectar diferencias.

---

## Tema: Planilla Electrónica — T-Registro y PLAME

1. ¿Qué información se registra en el T-Registro y qué se declara en el PLAME? Dé ejemplos concretos.
2. ¿Quiénes están obligados a llevar la Planilla Electrónica y cuál es su finalidad para SUNAT?
3. Describa el proceso general para declarar la planilla mensual mediante PDT PLAME.
4. Caso práctico: Un trabajador tiene ingresos extra por comisiones. Explique cómo se registran en T-Registro y cómo afectan la declaración PLAME.
5. ¿Qué controles se deben implementar para asegurar la calidad de los datos de la planilla antes de declararlos?
6. Explique las consecuencias de una declaración incorrecta en la planilla electrónica (sanciones, multas, ajustes retroactivos).
7. Diseñe un checklist para la revisión mensual de la planilla antes de la presentación al SUNAT.

---

## Tema: Herramientas contables y CONCAR (formatos Excel y registros)

1. Explique brevemente qué es CONCAR y en qué se diferencia de una hoja de cálculo para llevar registros contables.
2. ¿Qué ventajas ofrece el uso de plantillas Excel homologadas por SUNAT para registros contables?
3. Caso práctico: Explique los pasos para exportar desde CONCAR (o un ERP similar) un archivo compatible con PLE.
4. Diseñe una estructura de hoja de cálculo para el Registro de Compras que cumpla requisitos tributarios (campos, validaciones).
5. Explique cómo auditar asientos contables exportados desde CONCAR antes de subirlos al PLE.
6. Mencione tres buenas prácticas al trabajar con plantillas Excel para evitar errores al generar archivos para SUNAT.
7. Proponga una rutina automatizada (breve) para respaldar diariamente los archivos contables y el PLE.

---

## Tema: Integración, interoperabilidad y control interno

1. Defina interoperabilidad en el contexto de sistemas contables y SUNAT.
2. Explique por qué es importante la trazabilidad de los registros (quién, cuándo, qué) en los libros electrónicos.
3. Diseñe un flujo de trabajo que integre ventas e-commerce, plataforma de pagos y el sistema contable para alimentación automática del PLE.
4. Caso práctico: Identifica 5 controles clave que deberían existir para prevenir la emisión de comprobantes duplicados.
5. Explique cómo realizar una auditoría rápida de consistencia entre registros de ventas y libros electrónicos.
6. ¿Qué formatos de intercambio de datos (CSV, TXT, XML) son más comunes en PLE/SEE y para qué se usa cada uno?
7. Proponga una pauta de retención y archivado electrónico de comprobantes y libros (plazos, formato, accesos).

---

## Tema: Análisis de datos contables y KPIs

1. Mencione cinco KPIs financieros que pueden calcularse a partir de la base de datos contable y explique su utilidad.
2. Diseñe una consulta o fórmula básica para calcular el margen bruto mensual a partir de la base contable.
3. Explique cómo detectar anomalías en ventas usando técnicas simples (z-score, desviación estándar) sobre series mensuales.
4. Caso práctico: A partir de series mensuales de ventas y cuentas por cobrar, proponga un indicador de rotación de cartera y su fórmula.
5. ¿Cómo usaría dashboards (p. ej., Power BI o Google Data Studio) para apoyar la toma de decisiones contables? Describe dos visualizaciones clave.
6. Explique cómo preparar un dataset limpio desde el sistema contable para análisis en una herramienta de BI.
7. Proponga una pequeña batería de pruebas (sanity checks) que se ejecuten antes de publicar reportes financieros.

---

## Banco rápido: Preguntas de selección y V/F

1. V/F: El CUO es único por operación y por contribuyente. (Explique brevemente)
2. V/F: El SIRE reemplaza completamente al PLE en todos los escenarios. (Explique)
3. Opción múltiple: ¿Cuál NO es una ventaja de la emisión electrónica? a) Menor tiempo de archivado b) Reducción de errores c) Emisión sin conexión en todos los casos d) Mayor trazabilidad. (Respuesta correcta: c)
4. V/F: La Planilla Electrónica sólo la usa la SUNAT para fines estadísticos. (Explica)
5. Opción múltiple: ¿Qué formato es requerido con más frecuencia por el PLE? a) PDF b) TXT/CSV c) DOCX d) XLSX (Respuesta: b)
6. V/F: Una base de datos relacional usa relaciones para evitar la redundancia de datos. (Breve explicación)
7. Opción múltiple: ¿Cuál es un riesgo principal al aplicar IA en contabilidad? a) Mejora de eficiencia b) Sesgo en los datos c) Reducción de errores humanos d) Trazabilidad aumentada (Respuesta: b)

[[Banco de preguntas Solucionario]]

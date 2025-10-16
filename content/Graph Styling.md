---
dg-publish: false
tags: ["meta", "graph", "juggl", "css"]
---

# Estilado del Graph View y Juggl

Instrucciones y CSS para hacer el Graph View y la nube de tags más vistosa.

## Juggl

- Instala el plugin Juggl (mejor control de layouts y estilos de nodos).
- En Juggl, crea reglas para colorear nodos por tag, por ejemplo `tag: cursos` -> color.

## CSS (preview en Obsidian)

Puedes crear un archivo `obsidian.css` o pegar esto en tu snippet CSS en Obsidian (Settings -> Appearance -> CSS snippets).

```css
/* Tag chips para DataviewJS */
.tag-cloud-container {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}
.tag-cloud-container .tag-chip {
  padding: 6px 10px;
  border-radius: 8px;
  text-decoration: none;
  display: inline-block;
}

/* Opcional: resaltar backlinks y enlaces del hub */
.markdown-preview-view a.internal-link[href*="Plan de Estudios"] {
  background: linear-gradient(90deg, #fef3c7, #fee2b3);
  border-radius: 4px;
  padding: 2px 4px;
}
```

## Colores y reglas sugeridas

- `#ef4444` (rojo): temas urgentes / básicos
- `#3b82f6` (azul): finanzas/matemática
- `#10b981` (verde): inversiones/mercado

## Notas

- Algunos enlaces `obsidian://search` funcionan sólo dentro de la app Obsidian. Si abres las notas en un navegador esos enlaces no tendrán efecto.
- Juggl permite usar expresiones para agrupar por tag, crear leyendas, y fijar estilos por regla.

**_ Fin _**

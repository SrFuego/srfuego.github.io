---
dg-publish: false
tags: ["meta", "tags", "queries"]
dg-pinned: false
---

# Tags y consultas (Dataview)

Esta nota contiene ejemplos de consultas Dataview y DataviewJS que puedes pegar en Obsidian para explorar el gráfico y visualizar una nube de tags.

Ejemplo Dataview (lista simple de notas con tag `cursos`):

```dataview
table tags as "Tags", file.mtime as "Modificado"
from "content"
where contains(tags, "cursos")
sort file.mtime desc
```

Ejemplo DataviewJS: nube de tags (pequeño script que agrupa tags y muestra un tamaño relativo)

````dataviewjs
// Requiere Dataview y uso en Obsidian
const pages = dv.pages('"content"').where(p => p.tags && p.tags.includes('cursos'));
---
dg-publish: false
tags: ["meta", "tags", "queries"]
dg-pinned: false
---

# Tags y consultas (Dataview)

Esta nota contiene ejemplos de consultas Dataview y DataviewJS que puedes pegar en Obsidian para explorar el gráfico y visualizar una nube de tags.

Ejemplo Dataview (lista simple de notas con tag `cursos`):

```dataview
table tags as "Tags", file.mtime as "Modificado"
from "content"
where contains(tags, "cursos")
sort file.mtime desc
````

Ejemplo DataviewJS: nube de tags (pequeño script que agrupa tags y muestra un tamaño relativo)

```dataviewjs
// Requiere Dataview y uso en Obsidian
const pages = dv.pages('"content"').where(p => p.tags && p.tags.includes('cursos'));
const tagCounts = {};
for (let p of pages) {
  for (let t of p.tags) {
    tagCounts[t] = (tagCounts[t] || 0) + 1;
  }
}
// Palette de colores simple
const colors = ["#ef4444","#f59e0b","#10b981","#3b82f6","#8b5cf6","#ec4899","#06b6d4"];
const container = document.createElement('div');
container.className = 'tag-cloud-container';
for (let [tag, count] of Object.entries(tagCounts).sort((a,b)=>b[1]-a[1])) {
  const el = document.createElement('a');
  // link a búsqueda por tag en Obsidian (obsidian URI no funciona fuera de la app, pero clickable interna)
  el.setAttribute('href', `obsidian://search?query=%23${encodeURIComponent(tag)}`);
  el.className = 'tag-chip';
  el.textContent = `${tag} (${count})`;
  const size = 12 + Math.min(count, 10) * 3;
  el.style.fontSize = `${size}px`;
  const color = colors[Math.abs(hashCode(tag)) % colors.length];
  el.style.background = color + '22'; // light alpha
  el.style.border = `1px solid ${color}`;
  el.style.color = `${color}`;
  container.appendChild(el);
}
document.currentScript.parentElement.appendChild(container);

function hashCode(str) {
  let h = 0;
  for (let i = 0; i < str.length; i++) {
    h = (h << 5) - h + str.charCodeAt(i);
    h |= 0;
  }
  return h;
}
```

Consejos:

- Instala los plugins Dataview y Tag Wrangler (opcional) para enriquecer el manejo de tags.
- Usa Juggl o el Graph View de Obsidian para un gráfico más visual (Juggl permite layouts y agrupaciones avanzadas).

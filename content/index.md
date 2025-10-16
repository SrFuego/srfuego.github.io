# Bienvenido a mi Sitio de Finanzas

Hola mundo, soy SrFuego desde Quartz en Github Pages!

## Temas Principales

- [[Finanzas Personales]]
- [[Economía]]
- [[Inversiones]]
- [[Mercado de Valores]]
- [[Educación Financiera]]

## Notas Existentes

- [[Plan de Estudios]]
- [[Presupuesto y Finanzas Públicas]]
- [[Otra Prueba]]
- [[Prueba]]

las finanzas

## Cursos relacionados (Contabilidad y Finanzas)

Aquí un conjunto de notas creadas a partir del `Plan de Estudios`. Están pensadas para mejorar el gráfico de Obsidian y facilitar el enlace entre temas.

- [[Cursos de Contabilidad y Finanzas]]
- [[Matemática Financiera]]
- [[Fundamentos de Finanzas]]
- [[Contabilidad Financiera I]]
- [[Gestión y Control Financiero]]
- [[Mercado de Valores]]
- [[Presupuesto del Sector Público]]

### Nube de tags (DataviewJS)

Pega este bloque en Obsidian (requiere el plugin Dataview) para ver una nube de tags simple basada en las notas dentro de `content`:

```dataviewjs
const pages = dv.pages('"content"').where(p => p.tags && p.tags.includes('cursos'));
const tagCounts = {};
for (let p of pages) {
	for (let t of p.tags) {
		tagCounts[t] = (tagCounts[t] || 0) + 1;
	}
}
const palette = ["#ef4444","#f59e0b","#10b981","#3b82f6","#8b5cf6","#ec4899","#06b6d4"];
const container = document.createElement('div');
container.className = 'tag-cloud-container';
for (let [tag, count] of Object.entries(tagCounts).sort((a,b)=>b[1]-a[1])) {
	const el = document.createElement('a');
	el.setAttribute('href', `obsidian://search?query=%23${encodeURIComponent(tag)}`);
	el.className = 'tag-chip';
	el.textContent = `${tag} (${count})`;
	const size = 12 + Math.min(count, 10) * 3;
	el.style.fontSize = `${size}px`;
	const color = palette[Math.abs(hashCode(tag)) % palette.length];
	el.style.background = color + '22';
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

Si usas Juggl o el Graph View nativo, el hecho de tener muchas notas enlazadas y tags hará que el gráfico sea más denso e interesante.

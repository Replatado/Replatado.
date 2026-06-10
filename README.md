# Replatado 🌱

**Comida que vuelve a la mesa**

Landing page oficial de [Replatado](https://replatado.com) — emprendimiento de triple impacto creado en el programa *Aprender a Emprender* de Junior Achievement Argentina, colegio SI-SJP.

---

## ¿Qué hay en este repo?

| Archivo | Descripción |
|---|---|
| `index.html` | Landing page completa (todo en un archivo) |
| `logo.png` | Logo oficial 500×500px — no editar sin versión nueva |

---

## Cómo contribuir (para los 31 del equipo)

### 1. Cloná el repo
```bash
git clone https://github.com/[ORG]/replatado.git
cd replatado
```

### 2. Creá tu rama con tu nombre
```bash
git checkout -b fix/nombre-apellido
```
Ejemplos de nombres de rama:
- `fix/maria-gomez` → corrección pequeña
- `feature/maria-gomez` → algo nuevo
- `copy/maria-gomez` → cambios de texto

### 3. Hacé tus cambios en `index.html`

Abrí el archivo directamente en el navegador para ver cómo queda:
```
Doble click en index.html → se abre en Chrome/Firefox
```

### 4. Guardá y subí tu rama
```bash
git add index.html
git commit -m "Descripción corta de qué cambié"
git push origin fix/tu-nombre
```

### 5. Abrí un Pull Request en GitHub
- Entrá a github.com/[ORG]/replatado
- GitHub te va a mostrar un botón "Compare & pull request"
- Poné una descripción de qué cambiaste y por qué
- Asignalo al Director General para que apruebe

---

## Reglas básicas

- ✅ Siempre trabajar en tu propia rama, **nunca directamente en `main`**
- ✅ Un PR por cambio (no juntar 10 cosas distintas)
- ✅ Si cambiás el logo, coordinarlo con el equipo de Marketing
- ❌ No subir archivos pesados (fotos, videos) — usar links externos
- ❌ No tocar `logo.png` salvo versión oficial nueva

---

## Stack técnico

- HTML + CSS + JS vanilla (todo en `index.html`)
- Deploy automático en **Netlify** conectado a este repo
- Formulario via **Formspree** (ver sección de setup)
- Dominio: **replatado.com** (Namecheap → Netlify)

Cada vez que se aprueba un PR a `main`, Netlify redespliega automáticamente en menos de 1 minuto. 🚀

---

## Setup del formulario (solo quien administra)

El formulario de "Sumate como local" usa [Formspree](https://formspree.io):

1. Crear cuenta en formspree.io con el mail de Replatado
2. Crear nuevo formulario → copiar el ID (formato `xAbCdEfG`)
3. En `index.html`, buscar `REEMPLAZAR_ID` y cambiarlo por el ID real:
   ```html
   action="https://formspree.io/f/xAbCdEfG"
   ```
4. Las respuestas llegan al mail registrado en Formspree

---

## Equipo

Proyecto creado por estudiantes de SI-SJP en el marco de **Junior Achievement Argentina** — Aprender a Emprender 2025.

ODS: 🌍 2 (Hambre Cero) · ♻️ 12 (Consumo Responsable)

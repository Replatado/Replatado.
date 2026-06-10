# Guía rápida de Git para Replatado 🚀
## Para personas que nunca usaron Git

---

## Instalación

### Windows
1. Bajar **GitHub Desktop** desde https://desktop.github.com
2. Instalarlo y loguearse con tu cuenta de GitHub
3. Listo — no necesitás la terminal

### Mac
1. Bajar **GitHub Desktop** desde https://desktop.github.com
2. Instalarlo y loguearse
3. O usar la terminal (viene con Git instalado)

---

## Flujo con GitHub Desktop (más fácil)

### Primera vez
1. Abrí GitHub Desktop
2. `File → Clone repository`
3. Buscá `replatado` en la lista → `Clone`

### Para hacer un cambio
1. En GitHub Desktop → `Current Branch` → `New Branch`
2. Nombre: `fix/tu-nombre` (ej: `fix/lucas-perez`)
3. Clic en `Create Branch`
4. Abrí `index.html` con el Bloc de notas o VS Code y hacé tu cambio
5. En GitHub Desktop vas a ver el cambio en rojo/verde
6. Abajo a la izquierda: escribí un mensaje corto (ej: "Corregí typo en hero")
7. `Commit to fix/lucas-perez`
8. `Push origin` (botón azul arriba a la derecha)
9. `Create Pull Request` → se abre GitHub en el navegador
10. Poné descripción y mandalo

---

## Flujo con terminal

```bash
# Clonar (solo la primera vez)
git clone https://github.com/[ORG]/replatado.git
cd replatado

# Antes de empezar, traer los últimos cambios
git pull origin main

# Crear tu rama
git checkout -b fix/tu-nombre

# ... hacés tus cambios en index.html ...

# Ver qué cambiaste
git status
git diff

# Guardar cambios
git add index.html
git commit -m "Descripción de qué hice"

# Subir
git push origin fix/tu-nombre

# Ir a GitHub y abrir el Pull Request
```

---

## Preguntas frecuentes

**¿Perdí mis cambios?**
Si commiteaste, están guardados. Si no commiteaste, `git stash` los guarda temporalmente.

**¿Cómo veo los cambios de otros?**
`git pull origin main` desde la rama main trae todo lo nuevo.

**¿Me equivoqué en el commit message?**
`git commit --amend -m "Mensaje correcto"` (solo si no hiciste push todavía)

**¿Hay conflicto con otro cambio?**
Avisale al Director General o al encargado del repo para resolverlo juntos.

---

## VS Code (recomendado para editar HTML)

1. Bajar VS Code: https://code.visualstudio.com
2. `File → Open Folder` → elegir la carpeta `replatado`
3. Clic en `index.html` para editarlo
4. La extensión **Live Preview** (instalar desde el panel de extensiones) te muestra el resultado en tiempo real

---

¿Dudas? Escribir al grupo de WhatsApp del equipo de desarrollo 💬

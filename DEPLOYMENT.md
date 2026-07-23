# Deployment Paso a Paso

## Opción A: Usando GitHub Desktop (más fácil)

### 1. Descargar GitHub Desktop
- Ve a [github.com/apps/desktop](https://github.com/apps/desktop)
- Descarga e instala

### 2. Crear repo en GitHub
- Ve a [github.com/new](https://github.com/new)
- Nombre: `centro-operaciones`
- Descripción: "Centro de Operaciones — PWA"
- Public (para que Vercel pueda acceder)
- Crea el repo

### 3. Clonar y subir archivos
- Abre GitHub Desktop
- File → Clone Repository
- Selecciona `centro-operaciones`
- Copia los archivos de aquí a esa carpeta:
  - `index.html`
  - `manifest.json`
  - `service-worker.js`
  - `vercel.json`
  - `README.md`
  - `.gitignore`

### 4. Commit y Push
En GitHub Desktop:
- Tab "Changes"
- Escribe en "Summary": `Initial PWA commit`
- Click "Commit to main"
- Click "Push origin"

### 5. Conectar a Vercel
- Ve a [vercel.com](https://vercel.com) y loguéate con GitHub
- Click "Add New..." → "Project"
- Busca y selecciona `centro-operaciones`
- Click "Import"
- Espera 30 segundos
- ¡Listo! Tu link está en pantalla (ej: `centro-operaciones.vercel.app`)

---

## Opción B: Línea de comandos (si sabes Git)

```bash
# 1. Crear repo en GitHub.com manualmente (mismo que Opción A paso 2)

# 2. En tu máquina, en la carpeta con los archivos:
git init
git add .
git commit -m "Initial PWA"
git remote add origin https://github.com/TU_USUARIO/centro-operaciones.git
git branch -M main
git push -u origin main

# 3. Ve a Vercel.com → conecta GitHub → importa el repo
```

---

## En tu iPhone

Una vez tengas el link de Vercel (ej: `centro-operaciones.vercel.app`):

1. **Safari en iPhone**
2. Pega el link en la barra
3. Espera a que cargue
4. Tap en el botón "Compartir" (cuadrado con flecha)
5. Scroll down → "Añadir a pantalla de inicio"
6. Dale un nombre (ej: "Centro Ops")
7. Tap "Añadir"

¡Listo! Ya tienes la app en tu home con icono.

---

## Dominios personalizados

Si tienes un dominio (opcional):

1. Ve a Vercel → Project Settings → Domains
2. Añade tu dominio
3. Sigue las instrucciones de DNS

---

## Actualizaciones

Cada vez que hagas cambios:

```bash
# En tu máquina:
git add .
git commit -m "Cambios que hiciste"
git push

# Vercel auto-redeploy en 30 segundos
```

En el iPhone no necesitas hacer nada — la app se actualiza sola cuando abres Safari/refrescas.

---

**¿Preguntas?** Lee el README.md o ve a Vercel docs.

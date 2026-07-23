# Centro de Operaciones — PWA

App para iPhone. Un link, datos locales, funciona offline.

## Deployment (2 pasos)

### 1. Crear repo en GitHub

```bash
# En tu máquina:
git init
git add .
git commit -m "Initial PWA"
git remote add origin https://github.com/tu-usuario/centro-operaciones.git
git branch -M main
git push -u origin main
```

### 2. Conectar a Vercel

1. Ve a [vercel.com](https://vercel.com)
2. Conecta tu cuenta de GitHub
3. Importa el repo `centro-operaciones`
4. Vercel auto-detecta que es una PWA estática
5. **Deployment automático en 30 segundos**

Tu app vivirá en: `centro-operaciones.vercel.app` (o dominio personalizado)

---

## En tu iPhone

1. Abre Safari
2. Ve a `tu-app.vercel.app`
3. Tap "Compartir" → "Añadir a pantalla de inicio"
4. ¡Lista! Icono en home, funciona como app nativa

**Datos:** Todo se guarda en el iPhone (localStorage). No necesita backend.

---

## Cómo funciona

- **Sin backend:** Los datos viven en tu iPhone
- **Offline:** Funciona sin internet
- **Responsive:** Perfecta en celular
- **PWA:** Se instala como app nativa

---

## Datos

Cada día se guarda con la fecha. Acceso a 7 días anteriores en la pestaña SEMANA.

Los datos son tuyos, viven en tu teléfono. No se suben a ningún servidor.

---

**¿Problemas al hacer push a GitHub?**

```bash
# Si es la primera vez:
git config --global user.email "tu@email.com"
git config --global user.name "Tu Nombre"
```

**¿Vercel no detecta la PWA?**

Ve a Vercel → Settings → Build & Development → Deja "Framework" en "Other"

---

**Listo. A usar en el iPhone. 💪**

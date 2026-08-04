# Publicar liftlog-legal en GitHub Pages

Guía paso a paso (primera vez).

## 1. Crear el repositorio en GitHub

1. Abre https://github.com/new
2. **Repository name:** `liftlog-legal`
3. **Public**
4. No marques «Add a README» (ya tienes archivos locales)
5. Clic en **Create repository**

## 2. Subir este directorio

En PowerShell, desde `Desktop\liftlog-legal`:

```powershell
git init
git branch -M main
git add -A
git commit -m "Sitio legal LiftLog (privacidad, términos, aviso legal)"
git remote add origin https://github.com/pedrobornes/liftlog-legal.git
git push -u origin main
```

Si el repo ya existe con commits, usa solo `git push -u origin main`.

## 3. Activar GitHub Pages

1. Repo → **Settings** → **Pages**
2. **Build and deployment** → Source: **Deploy from a branch**
3. Branch: `main` → folder: `/ (root)` → **Save**
4. Espera 1–2 minutos. La URL será:

   **https://pedrobornes.github.io/liftlog-legal/**

## 4. Verificar

Abre en el navegador:

- https://pedrobornes.github.io/liftlog-legal/privacy.html
- https://pedrobornes.github.io/liftlog-legal/terms.html
- https://pedrobornes.github.io/liftlog-legal/legal.html

## 5. Conectar la app

Copia las variables de `README.md` a `liftlog/frontend/.env` y reinicia Vite.

## Google Play (más adelante)

- **Política de privacidad:** URL de `privacy.html`
- **Data safety:** coherente con la política (email, entrenos, eliminación de cuenta en app)

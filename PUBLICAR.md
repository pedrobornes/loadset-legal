# Publicar loadset-legal en GitHub Pages

Guía paso a paso (primera vez o tras renombrar desde liftlog-legal).

## 1. Renombrar el repositorio en GitHub (si aún se llama liftlog-legal)

1. Abre https://github.com/pedrobornes/liftlog-legal → **Settings** → **General**
2. **Repository name:** `loadset-legal` → **Rename**
3. En local (desde `Desktop\loadset-legal`):

```powershell
git remote set-url origin https://github.com/pedrobornes/loadset-legal.git
```

## 2. Si creas el repo desde cero

1. Abre https://github.com/new
2. **Repository name:** `loadset-legal`
3. **Public**
4. No marques «Add a README»
5. Clic en **Create repository**

```powershell
cd $env:USERPROFILE\Desktop\loadset-legal
git remote add origin https://github.com/pedrobornes/loadset-legal.git
git push -u origin main
```

## 3. Activar / comprobar GitHub Pages

1. Repo → **Settings** → **Pages**
2. Source: **Deploy from a branch** → `main` → `/ (root)` → **Save**
3. URL:

   **https://pedrobornes.github.io/loadset-legal/**

## 4. Verificar

- https://pedrobornes.github.io/loadset-legal/privacy.html
- https://pedrobornes.github.io/loadset-legal/terms.html
- https://pedrobornes.github.io/loadset-legal/legal.html

## 5. Conectar la app

Las variables en `loadset/frontend/.env` ya deben apuntar a `loadset-legal`. Reinicia Vite / haz `cap:sync` si hace falta.

## Google Play (más adelante)

- **Política de privacidad:** URL de `privacy.html`
- **Data safety:** coherente con la política

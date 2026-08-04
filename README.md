# liftlog-legal

Documentos legales públicos de **LiftLog** (GitHub Pages).

**Titular:** Pedro Antonio Bornes Durán  
**Contacto:** info@status-timer.com

## URLs publicadas

| Documento | URL |
|-----------|-----|
| Índice | https://pedrobornes.github.io/liftlog-legal/ |
| Privacidad | https://pedrobornes.github.io/liftlog-legal/privacy.html |
| Términos | https://pedrobornes.github.io/liftlog-legal/terms.html |
| Aviso legal | https://pedrobornes.github.io/liftlog-legal/legal.html |

## Configuración en la app LiftLog

En `liftlog/frontend/.env`:

```env
VITE_LEGAL_PRIVACY_URL=https://pedrobornes.github.io/liftlog-legal/privacy.html
VITE_LEGAL_TERMS_URL=https://pedrobornes.github.io/liftlog-legal/terms.html
VITE_LEGAL_NOTICE_URL=https://pedrobornes.github.io/liftlog-legal/legal.html
VITE_LEGAL_CONTACT_EMAIL=info@status-timer.com
```

## Editar datos

1. Modifica `legal.config.json` (referencia local; los HTML ya están rellenados).
2. Si cambias textos, edita los `.html` directamente.
3. Antes de monetizar: revisa textos con un profesional si cambias el modelo de negocio.

## Publicar cambios

```bash
git add -A
git commit -m "Actualizar textos legales"
git push
```

GitHub Pages sirve automáticamente desde `main` (unos segundos de delay).

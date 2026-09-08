# J&C Imports

Sitio web de perfumes árabes y reservas de cortes de pelo.

## Archivos necesarios

- `index.html` → página principal
- `audio.mp3` → pista de ambiente (se reproduce al entrar)

Ambos archivos deben estar en la **raíz** del repositorio (mismo nivel).

## Cómo subirlo a GitHub (sin problemas)

### Opción 1 — Desde la web de GitHub (más fácil)

1. Entrá a [github.com](https://github.com) e iniciá sesión.
2. Clic en **New repository**.
3. Nombre del repo (ejemplo: `jc-imports` o `jcimports`).
4. Dejá **Public**.
5. **No** marques “Add a README” (ya tenés uno).
6. Create repository.
7. En la página del repo vacío, arrastrá los dos archivos (`index.html` y `audio.mp3`) o usá “uploading an existing file”.
8. Commit changes.

### Activar GitHub Pages

1. En el repo → **Settings** → **Pages** (menú izquierdo).
2. Source: **Deploy from a branch**.
3. Branch: `main` (o `master`) → carpeta `/ (root)`.
4. Save.
5. Esperá 1–2 minutos. La URL queda:
   `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`

### Opción 2 — Con Git en la terminal

```bash
# 1. Creá una carpeta y meté los archivos
mkdir jc-imports
cd jc-imports
# (copiá index.html y audio.mp3 acá)

# 2. Inicializá git
git init
git add index.html audio.mp3 README.md
git commit -m "Sitio J&C Imports listo"

# 3. Creá el repo vacío en GitHub (sin README) y después:
git branch -M main
git remote add origin https://github.com/TU-USUARIO/NOMBRE-DEL-REPO.git
git push -u origin main
```

Después activá Pages como arriba.

## Notas importantes

- El archivo de audio **tiene que llamarse exactamente** `audio.mp3` (o cambiá el `src` en el HTML).
- No uses subcarpetas para estos dos archivos si querés que funcione de una.
- Mercado Pago: reemplazá `https://mpago.la/TU-LINK` por tu link real.
- Alias bancario: si tenés uno, ponelo en `DATOS_TRANSFERENCIA.alias`.
- Supabase (turnos compartidos): opcional. Si no configurás nada, los turnos se guardan solo en el navegador del cliente.

## Vista previa local

Abrí `index.html` en el navegador. Si el audio no arranca solo (política del navegador), tocá el botón play del reproductor de abajo.

# FOMO — página inicial

Página estática, responsive y sin dependencias externas, preparada para publicarse gratis mediante GitHub Pages.

## Estructura

```text
fomo-landing-page/
├── index.html
├── .nojekyll
├── README.md
└── assets/
    ├── fomo-logo.svg
    ├── fomo-icon.svg
    ├── favicon.png
    ├── byma-logo.png
    └── cafci-logo.png
```

## Antes de publicar: reemplazar los logos de las fuentes

Los archivos `assets/byma-logo.png` y `assets/cafci-logo.png` incluidos en este paquete son marcadores provisorios.

1. Conseguí las imágenes que vas a utilizar y verificá que contás con autorización para mostrarlas.
2. Recortá el espacio vacío sobrante de cada imagen.
3. Usá preferentemente PNG con fondo transparente.
4. Renombrá los archivos exactamente así:
   - `byma-logo.png`
   - `cafci-logo.png`
5. Reemplazá los dos archivos existentes dentro de la carpeta `assets`.

No hace falta modificar el HTML si se conservan esos nombres.

## Vista previa en tu computadora

La forma más simple es abrir `index.html` con el navegador.

Para una prueba más parecida a un sitio publicado, abrí una terminal dentro de la carpeta y ejecutá:

```bash
python -m http.server 8000
```

Después visitá:

```text
http://localhost:8000
```

Para detener el servidor, presioná `Ctrl + C`.

## Publicación mediante GitHub Pages usando el navegador

### 1. Crear el repositorio

1. Iniciá sesión en GitHub.
2. En la esquina superior derecha, presioná `+` y elegí **New repository**.
3. En **Repository name**, escribí `fomo-landing`.
4. Agregá una descripción, por ejemplo: `Página inicial del proyecto FOMO`.
5. Elegí **Public** para utilizar GitHub Pages con una cuenta gratuita.
6. No agregues otro README, `.gitignore` ni licencia: el paquete ya contiene lo necesario.
7. Presioná **Create repository**.

### 2. Subir los archivos

1. Dentro del repositorio nuevo, elegí **Add file → Upload files**.
2. Abrí la carpeta descomprimida en tu computadora.
3. Arrastrá al navegador el archivo `index.html`, el archivo `README.md`, el archivo `.nojekyll` y la carpeta `assets`.
4. Verificá que `index.html` quede en la raíz del repositorio y no dentro de otra carpeta.
5. En **Commit changes**, escribí `Publicar primera página de FOMO`.
6. Elegí **Commit directly to the main branch** y confirmá.

### 3. Activar GitHub Pages

1. Abrí **Settings** dentro del repositorio.
2. En la barra lateral, elegí **Pages**.
3. En **Build and deployment**, seleccioná **Deploy from a branch**.
4. En **Branch**, elegí `main` y la carpeta `/ (root)`.
5. Presioná **Save**.
6. Esperá unos minutos y volvé a esa sección. GitHub mostrará la dirección publicada.

La URL tendrá esta forma:

```text
https://TU-USUARIO.github.io/fomo-landing/
```

## Actualizar el sitio más adelante

### Cambiar texto

1. Abrí `index.html` en GitHub.
2. Presioná el ícono del lápiz.
3. Modificá el contenido.
4. Presioná **Commit changes**.

GitHub Pages volverá a publicar automáticamente la nueva versión.

### Reemplazar un logo

1. Entrá a la carpeta `assets` del repositorio.
2. Eliminá el archivo anterior o subí un archivo nuevo con exactamente el mismo nombre.
3. Confirmá el cambio mediante un commit.

## Opción de URL más corta

Para que la página principal de tu cuenta sea:

```text
https://TU-USUARIO.github.io/
```

el repositorio debe llamarse exactamente:

```text
TU-USUARIO.github.io
```

En ese caso, seguí el mismo procedimiento de carga y publicación.

## Dominio propio, más adelante

GitHub Pages permite conectar un dominio propio desde **Settings → Pages → Custom domain**. Conviene verificar primero el dominio dentro de la configuración de la cuenta de GitHub y luego configurar los registros DNS con el proveedor del dominio.

## Recomendaciones

- No subas contraseñas, claves de API ni información privada al repositorio.
- Conservá `index.html` en la raíz.
- Conservá la carpeta `assets` y sus nombres.
- Probá la página en un teléfono antes de difundirla.
- Confirmá las condiciones de uso de los logos y de los datos antes del lanzamiento público.

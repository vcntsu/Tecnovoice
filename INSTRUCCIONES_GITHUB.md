# 📦 Cómo subir TecnoVoice a GitHub Pages

## Paso 1: Crear repositorio en GitHub

1. Ve a https://github.com/new
2. Nombre del repositorio: `TecnoVoice`
3. Descripción: `Calculadora financiera por voz`
4. Público
5. Click en "Create repository"

## Paso 2: Subir el código

### Opción A: Desde la terminal (recomendado)

```bash
# Inicializar git en tu carpeta
cd C:/Users/vicen/OneDrive/Escritorio/TecnoVoice
git init

# Agregar todos los archivos
git add .

# Hacer commit
git commit -m "Primera versión de TecnoVoice"

# Conectar con GitHub (reemplaza TU-USUARIO)
git remote add origin https://github.com/TU-USUARIO/TecnoVoice.git

# Subir
git branch -M main
git push -u origin main
```

### Opción B: Desde GitHub Desktop (más fácil)

1. Descarga GitHub Desktop: https://desktop.github.com/
2. Instala y abre GitHub Desktop
3. File → Add Local Repository
4. Selecciona la carpeta `TecnoVoice`
5. Click en "Publish repository"
6. Marca "Public" y click en "Publish"

### Opción C: Subir archivos manualmente

1. Ve a tu repositorio en GitHub
2. Click en "uploading an existing file"
3. Arrastra todos los archivos de la carpeta TecnoVoice
4. Click en "Commit changes"

## Paso 3: Activar GitHub Pages

1. En tu repositorio, ve a **Settings** (⚙️)
2. En el menú izquierdo, click en **Pages**
3. En "Source", selecciona **main** branch
4. Click en **Save**
5. Espera 1-2 minutos

## Paso 4: Obtener tu URL

Verás un mensaje:
```
Your site is published at https://TU-USUARIO.github.io/TecnoVoice/
```

¡Esa es tu URL! Ábrela en tu móvil.

## 🎉 ¡Listo!

Ahora puedes:
- Abrir la URL en tu móvil
- Compartirla con quien quieras
- El reconocimiento de voz funcionará perfectamente

## 🔄 Actualizar el código

Cada vez que hagas cambios:

```bash
git add .
git commit -m "Descripción del cambio"
git push
```

Los cambios aparecerán en 1-2 minutos en tu sitio.

## ⚡ Alternativa rápida: Netlify

Si no quieres usar GitHub:

1. Ve a https://app.netlify.com/drop
2. Arrastra la carpeta `TecnoVoice`
3. Te da una URL HTTPS instantánea
4. ¡Listo!

## 🆘 Problemas comunes

### "Permission denied"
```bash
# Configura tu usuario de GitHub
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

### "Repository not found"
Verifica que la URL sea correcta:
```bash
git remote -v
```

### No aparece en GitHub Pages
- Espera 2-3 minutos
- Verifica que el archivo se llame `index.html` o esté en la raíz
- Revisa que GitHub Pages esté activado en Settings

## 📱 Probar en móvil

1. Abre la URL de GitHub Pages en tu móvil
2. Presiona el micrófono
3. Permite el acceso
4. ¡Habla!

**Importante:** La URL debe empezar con `https://` (GitHub Pages lo hace automáticamente)

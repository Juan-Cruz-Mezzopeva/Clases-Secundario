# 🚀 Guía Paso a Paso: Sube tu Primera Web a GitHub

¡Felicitaciones! Ya armaste la estructura de tu página con HTML (los cimientos y paredes) y le diste estilo con CSS. Ahora vamos a usar nuestro superpoder, la **máquina del tiempo** llamada Git, para guardar este trabajo de forma segura y "empujarlo" a la nube para que cualquiera pueda visitarlo. 

Sigue estos pasos con cuidado. ¡Estás trabajando como un desarrollador profesional!

---

## ☁️ Fase 1: Crear el espacio en la nube (GitHub)

Antes de mandar los archivos, necesitamos decirle a GitHub que nos prepare una caja vacía para recibirlos.

1. Entra a tu cuenta en [GitHub](https://github.com/).
2. Arriba a la derecha, haz clic en el botón verde **"New"** (o en el símbolo `+` y luego "New repository").
3. En **Repository name**, ponle un nombre a tu proyecto (por ejemplo: `mi-primer-sitio-web`). *Trata de no usar espacios, usa guiones cortos.*
4. Déjalo en **Public** (Público).
5. ⚠️ **¡Súper importante!** NO marques ninguna casilla de abajo (ni "Add a README", ni `.gitignore`). Queremos la caja totalmente vacía.
6. Haz clic en el botón verde **"Create repository"**. 

Te va a aparecer una pantalla con muchas instrucciones y un link. ¡Déjala abierta, la vamos a usar en un minuto!

---

## 💻 Fase 2: Preparar la foto local (En tu computadora)

Ahora vamos a tu computadora, a la carpeta donde creaste tu archivo `index.html` y tus estilos.

1. Abre tu terminal (**Git Bash**).
2. Usa el comando `cd` para ingresar a la carpeta de tu proyecto. (Ejemplo: `cd proyectodds`).
3. Si es la primera vez en esa carpeta, dile a Git que empiece a observar los archivos escribiendo:
   ```bash
   git init
El Chismoso: Escribe git status. Vas a ver tus archivos index.html y CSS en color rojo. Eso significa que Git los ve, pero todavía no los está siguiendo.
A la tarima: Vamos a preparar todos los archivos para la foto. Escribe el siguiente comando (¡no te olvides del punto al final!). Esto pasa los archivos al área de Staging (color verde).
La foto fija: Llegó el momento de sacar la foto y guardarla en tu historial con un mensaje obligatorio.

--------------------------------------------------------------------------------
## 🚀 Fase 3: ¡El gran empuje a la Nube!

Ya tienes la foto guardada en tu compu, ahora hay que mandarla a la caja vacía que creaste en GitHub.
Vuelve a la pestaña de GitHub que dejaste abierta en la Fase 1. Busca la sección que dice "…or push an existing repository from the command line" y copia las 3 líneas de código que te aparecen ahí. Pégalas de a una en tu consola y presiona Enter.
Se verán más o menos así:
- Le damos nombre a la rama principal:
- Conectamos tu compu con la nube (pega tu propio link aquí):
- El gran empuje final: Sube tu historial y tus archivos a GitHub.

🎉 ¡LISTO! Vuelve a tu página de GitHub y recarga la pestaña (F5). ¡Vas a ver tu código index.html y tus carpetas subidas en la nube! Acabas de completar el flujo de trabajo estándar de la industria tecnológica global.

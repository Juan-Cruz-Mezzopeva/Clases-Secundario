# 🚀 Guía Paso a Paso: Crea y Sube tu Proyecto a GitHub

Esta guía te muestra cómo crear un repositorio en GitHub, configurarlo en tu equipo y subir un proyecto local al repositorio remoto.

---

## 1. Antes de comenzar: requisitos

- Tener una cuenta en GitHub.
- Tener instalado Git en tu computadora.
- Tener tu proyecto local listo: carpeta con `index.html`, `style.css` u otros archivos.
- Usar Git Bash o la terminal que prefieras.

---

## 2. Configurar Git en tu equipo

Abre Git Bash y ejecuta estos comandos solo si nunca configuraste Git en esta computadora:

```bash
git config --global user.name "Tu Nombre Apellido"
git config --global user.email "tu@email.com"
```

Esto permite a Git identificar tus cambios.

Para verificar la configuración:

```bash
git config --global --list
```

---

## 3. Crear el repositorio remoto en GitHub

1. Ingresa a tu cuenta de GitHub.
2. Haz clic en el botón `New` o en el ícono `+` y luego en `New repository`.
3. Completa los campos:
   - `Repository name`: un nombre corto y claro, por ejemplo `mi-primer-sitio-web`.
   - `Description` (opcional): una breve descripción.
   - `Public` o `Private` según prefieras.
4. NO marques ninguna casilla de abajo: no agregues `README`, `.gitignore` ni `license`.
5. Haz clic en `Create repository`.

GitHub te mostrará una página con instrucciones y comandos para conectar tu carpeta local.

---

## 4. Iniciar Git en tu proyecto local

En Git Bash, entra en la carpeta de tu proyecto:

```bash
cd ruta/a/tu/proyecto
```

Inicia el repositorio local:

```bash
git init
```

Verifica el estado actual:

```bash
git status
```

Deberías ver tus archivos sin seguimiento en rojo.

---

## 5. Agregar archivos al área de preparación (staging)

Prepara todos los archivos del proyecto para el primer commit:

```bash
git add .
```

Comprueba el estado otra vez:

```bash
git status
```

Ahora los archivos aparecerán en verde como listos para confirmar.

---

## 6. Crear el primer commit

Guarda un registro de tu trabajo con un mensaje claro:

```bash
git commit -m "Primer commit: subo el proyecto inicial"
```

Esto crea una instantánea de tu proyecto en tu equipo.

---

## 7. Conectar el repositorio local con GitHub

En la página del repositorio remoto en GitHub, copia las instrucciones bajo el título `…or push an existing repository from the command line`.

Generalmente son tres comandos como estos:

```bash
git branch -M main
git remote add origin https://github.com/tu-usuario/mi-primer-sitio-web.git
git push -u origin main
```

- `git branch -M main` renombra tu rama principal a `main`.
- `git remote add origin ...` conecta tu carpeta local con el repositorio remoto.
- `git push -u origin main` sube tu primer commit a GitHub.

---

## 8. Verificar en GitHub

1. Regresa a la página del repositorio en GitHub.
2. Recarga la página (F5).
3. Verifica que tus archivos (`index.html`, `style.css`, etc.) estén visibles.

¡Felicidades! Ya tienes tu proyecto en GitHub.

---

## 9. Flujo básico para futuros cambios

Cada vez que hagas cambios, usa estos comandos:

```bash
git add .
git commit -m "Descripción corta del cambio"
git push
```

Así guardas los cambios localmente y los subes al repositorio remoto.

---

## 10. Consejos útiles

- Usa mensajes de commit claros, por ejemplo: `Arregla diseño del menú`.
- Revisa `git status` antes de cada commit.
- Si necesitas ver el historial, usa `git log`.
- Para descargar los cambios del remoto en el futuro, usa `git pull`.

---

## Resumen rápido

1. Configura Git con tu nombre y correo.
2. Crea un repositorio vacío en GitHub.
3. Dentro de tu proyecto local, usa `git init`, `git add .`, y `git commit`.
4. Conecta el remoto con `git remote add origin ...`.
5. Sube todo con `git push -u origin main`.

¡Listo! Tu proyecto local ya está en GitHub y puedes continuar trabajando como un desarrollador real.

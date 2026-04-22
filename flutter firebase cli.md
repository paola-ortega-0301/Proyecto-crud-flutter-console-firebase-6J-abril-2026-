¡Excelente elección! Combinar Flutter con Firebase es como darle superpoderes a tu app. Para que todo funcione sobre ruedas, necesitamos preparar tu entorno de desarrollo.

Aquí tienes la guía paso a paso para configurar Node.js y las herramientas de Firebase.

---

## 1. Software necesario: Node.js y npm
Para instalar el Firebase CLI, necesitas **Node.js**, que es un entorno de ejecución para JavaScript. Al instalar Node.js, se incluye automáticamente **npm** (Node Package Manager), que es la herramienta que usaremos para descargar Firebase.

### Cómo verificar si ya los tienes
Antes de instalar nada, abre tu terminal (PowerShell en Windows, Terminal en macOS/Linux) y ejecuta:

* **Para Node.js:** `node -v`
* **Para npm:** `npm -v`

> Si ves un número de versión (ej. `v20.10.0`), ¡ya estás listo! Si recibes un error de "comando no encontrado", sigue los pasos de abajo.

---

## 2. Instalación de Node.js paso a paso
Si no lo tienes instalado, sigue estos pasos para asegurar una instalación limpia y global:

1.  **Descarga:** Ve al sitio oficial [nodejs.org](https://nodejs.org/).
2.  **Versión recomendada:** Elige la versión **LTS** (Long Term Support). Es la más estable para desarrollo.
3.  **Instalador:** Ejecuta el archivo descargado (`.msi` en Windows o `.pkg` en macOS).
4.  **Configuración:** Dale a "Next" en todo. Asegúrate de que la casilla **"Add to PATH"** esté marcada (esto es lo que permite que funcione de manera "global").
5.  **Finalizar:** Reinicia tu terminal o computadora para que los cambios surtan efecto.

---

## 3. Instalación de Firebase CLI (firebase-tools)
Una vez que `npm` esté funcionando, instalaremos las herramientas de Firebase. El parámetro `-g` es fundamental, ya que indica que la instalación es **global**.

### El comando mágico:
Ejecuta esto en tu terminal:
```bash
npm install -g firebase-tools
```

* **¿Qué hace esto?** Descarga el paquete `firebase-tools` y lo registra en tu sistema para que puedas usar el comando `firebase` desde cualquier carpeta de tus proyectos.

---

## 4. Acceso a Firebase con Google
Ahora que tienes las herramientas, debes vincular tu terminal con tu cuenta de Google para que Firebase sepa quién eres y a qué proyectos tienes acceso.

### Comando de Login:
```bash
firebase login
```

**¿Qué sucederá?**
1.  La terminal te preguntará si quieres permitir que Firebase recopile información de error (puedes decir `Y` o `N`).
2.  Se abrirá automáticamente tu **navegador web**.
3.  Selecciona tu cuenta de Google.
4.  Haz clic en **"Permitir"**.
5.  Verás un mensaje en el navegador que dice: *"Firebase CLI Login Successful"*.

---

## 5. Bonus: Preparar Flutter para Firebase
Aunque ya tienes el CLI de Firebase, para Flutter se recomienda usar **FlutterFire CLI**, que automatiza la configuración de archivos nativos.

Una vez logueado en Firebase, ejecuta este comando para instalar la herramienta específica de Flutter:
```bash
dart pub global activate flutterfire_cli
```

### Comandos útiles para recordar:
| Tarea | Comando |
| :--- | :--- |
| Ver versión de Firebase | `firebase --version` |
| Cerrar sesión | `firebase logout` |
| Listar tus proyectos | `firebase projects:list` |
| Configurar FlutterFire | `flutterfire configure` |

---

¿Ya lograste ver la versión de Node en tu terminal o prefieres que revisemos algún error específico que te haya salido?

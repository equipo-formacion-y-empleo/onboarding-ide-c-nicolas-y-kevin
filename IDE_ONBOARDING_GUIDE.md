# Guía de Configuración de Entornos de Desarrollo

> 📋 **Guía Técnica**: Esta documentación establece los procedimientos para configurar un entorno de desarrollo en C# y otros lenguajes. Incluye las configuraciones necesarias para mantener consistencia en el desarrollo de software.

> **Nota importante**: Este documento se enfoca en aspectos técnicos y procedimientos. Para análisis comparativos, reflexiones personales y conclusiones, utiliza el archivo `CONCLUSIONES_EVALUACION.md`.

**Autores**: [Nicolas] y [Kevin]
**Fecha V0**: [Fecha de entrega inicial]
**Fecha V1**: [Fecha de entrega final]

---

## Visual Studio Code - Entorno Principal

### Instalación y Verificación

#  Método de Instalación de Visual Studio Code

## 1. Acceder al sitio oficial
Dirígete al sitio web oficial de Visual Studio Code:
[https://code.visualstudio.com](https://code.visualstudio.com)
![Imagen_Enlace_VSCode](screenshots/VSCode_enlace.png)

---

## 2. Seleccionar el sistema operativo
Haz clic en el botón de descarga correspondiente a tu sistema operativo:

- **Windows**
- **macOS**
- **Linux**

![Sistemas operativos posibles](screenshots/VSCode_SistemaOperativo.png)

---

## 3. Descargar el instalador
Esto dependiendo de tu sistema operativo, se descargará uno de los siguientes archivos:

- `.exe` para **Windows** *"En nuestro caso"*
- `.dmg` para **macOS**
- `.deb` o `.rpm` para **Linux**

![En nuestro caso ".exe" y estamos en Windows](screenshots/VSCode_Archivo.png)

---

## 4. Instalar Visual Studio Code

### Para Windows
1. Ejecuta el archivo `.exe`.
2. Acepta los términos de licencia.
3. Elige la carpeta de instalación.
4. Opcional: activa las opciones como:
   - "Agregar al PATH"
   - "Crear accesos directos"
5. Haz clic en **Instalar**.
6. Al finalizar, haz clic en **Finalizar** para abrir VS Code.

---

### Para macOS
1. Abre el archivo `.dmg`.
2. Arrastra el ícono de **Visual Studio Code** a la carpeta **Aplicaciones**.
3. *(Opcional)* Para abrir VS Code desde la terminal:
   - Abre VS Code
   - Presiona `Cmd + Shift + P`
   - Escribe `Shell Command: Install 'code' command in PATH` y selecciona la opción.

---

### Para Linux

#### Para distribuciones Debian/Ubuntu (.deb)

sudo dpkg -i nombre-del-archivo.deb
sudo apt-get install -f  # Para corregir dependencias si es necesario

### Uso Básico de VS Code

**Navegación y funcionalidades básicas:**
- Navegación por la interfaz
- Edición de código
- Uso de la paleta de comandos
- Gestión de archivos y carpetas

### Personalización del Entorno

**Configuraciones aplicadas:** [Describir las personalizaciones que se realizaron]

*Ejemplos de configuraciones útiles (elegir las que se consideren relevantes):*

**Temas e iconos:**
Ejemplos:
- Material Theme, One Dark Pro
- File Icon Theme para mejor identificación de archivos

**Configuración de fuentes:**
Ejemplos:
- Fira Code, JetBrains Mono (con ligaduras)

**Atajos de teclado útiles:**
Ejemplos:
- Ctrl+/ para comentar/descomentar
- Ctrl+Shift+P para paleta de comandos
- Ctrl+` para terminal integrada
- Alt+↑/↓ para mover líneas

**Configuración del editor:**
Ejemplos:
- Formateo automático al guardar
- Detección automática de indentación
- Word wrap para líneas largas

**Terminal integrada:**
Ejemplos:
- PowerShell como terminal predeterminado
- Configuración de perfil personalizado

> **Personaliza según tus necesidades**: Estas son sugerencias basadas en prácticas comunes. Experimenta y documenta las configuraciones que encuentres más útiles para tu flujo de trabajo.> 💼 **Manual de Incorporación**: Esta guía establece los estándares del equipo para configurar entornos de desarrollo en C#. Cualquier nuevo desarrollador debe poder seguir estas instrucciones para configurar su entorno de trabajo de manera consistente con el resto del equipo.

### SDK .NET

**Proceso de instalación:**
1. **Descarga e instalación:** [Describir el proceso]
2. **Verificación:** [Cómo comprobar que funciona]

### Configuración para C#

**Extensiones esenciales:**
- **Soporte oficial para C#**: Extensión que proporciona IntelliSense, debugging y compilación


**Configuraciones específicas para C#:** 
[Describir las configuraciones que se aplicaron, como formateo automático, intellisense, o configuraciones del compilador]

**Debugging básico:**
- Configuración de puntos de interrupción (breakpoints)
- Ejecutar y depurar
- Inspección de variables

> **Enfoque práctico**: Concentra tu documentación en las funcionalidades básicas que usarás día a día.

### Flujo de Trabajo con C#

**Creación de proyectos:**
[Documentar el proceso para crear proyectos C#]

**Estructura de proyecto:**
```csharp
// Incluir aquí un ejemplo del código desarrollado
// Comentarios sobre las decisiones tomadas
```

**Compilación y ejecución:**
[Proceso para compilar y ejecutar proyectos]

**Debugging:**
[Configuración y uso de debugging]

---

## Visual Studio - IDE Alternativo

### Instalación

**Proceso de instalación:**
- **Descarga:** [Versión recomendada - Community/Professional]
- **Componentes necesarios:** [Componentes específicos para C#]
- **Verificación:** [Cómo confirmar instalación correcta]

### Desarrollo con C#

**Creación de proyecto:**
[Describir el proceso para crear un proyecto C# en Visual Studio]

**Flujo de trabajo básico:**
- Compilación y ejecución
- Uso de Solution Explorer
- Debugging básico

---

## Configuración de Lenguaje Adicional

**Lenguaje seleccionado:** [Java/Python/Otro] - **Justificación:** [Por qué se eligió este lenguaje]

### Instalación del Entorno

**Runtime/SDK:**
- **Descarga e instalación:** [Proceso paso a paso]
- **Verificación:** [Cómo confirmar que funciona]

### Configuración en VS Code

**Extensiones por lenguaje:**

*Para Java:*
- **Paquete completo de Java**: Incluye compilación, debugging y gestión de proyectos

*Para Python:*
- **Soporte oficial de Python**: Extensión completa con intérprete y debugging

*Para otros lenguajes:*
- Busca la extensión oficial del lenguaje que proporcione soporte completo

**Configuraciones específicas aplicadas:**
[Documentar los ajustes que se realizaron, como configuración del intérprete, formateo automático, linting, etc.]

### Proyecto de Ejemplo

**Código desarrollado:**
```[lenguaje]
// Código de ejemplo aquí
// Comentarios explicativos
```

**Proceso de ejecución:**
[Describir cómo ejecutar el código]

---

## Configuraciones Recomendadas

**Configuraciones generales:**
[Documentar configuraciones que se consideran útiles para cualquier desarrollador]

**Herramientas adicionales:**
[Extensions, herramientas CLI, o utilidades que se consideran beneficiosas]

**Solución de problemas comunes:**
[Problemas frecuentes durante la configuración y sus soluciones]

**Recursos útiles:**
- Enlace [Enlace]: [Descripción]
- Documentación [Documentación]: [Descripción]

---

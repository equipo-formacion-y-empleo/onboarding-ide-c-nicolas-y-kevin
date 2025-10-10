# Guía de Configuración de Entornos de Desarrollo

> 📋 **Guía Técnica**: Esta documentación establece los procedimientos para configurar un entorno de desarrollo en C# y otros lenguajes. Incluye las configuraciones necesarias para mantener consistencia en el desarrollo de software.

> **Nota importante**: Este documento se enfoca en aspectos técnicos y procedimientos. Para análisis comparativos, reflexiones personales y conclusiones, utiliza el archivo `CONCLUSIONES_EVALUACION.md`.

**Autores**: [Nombre 1] y [Nombre 2]
**Fecha V0**: [Fecha de entrega inicial]
**Fecha V1**: [Fecha de entrega final]

---

## Visual Studio Code - Entorno Principal

### Instalación y Verificación

**Método de instalación:** [Especifica el método recomendado]

> **💡 Sobre las imágenes**: Incluye capturas de pantalla para mostrar los diferentes pasos o resultados. Ejemplo: ![Descripción clara del contenido](screenshots/placeholder.png)`

**Proceso de instalación:**
- **Descarga:** [Describir el proceso]
- **Opciones del instalador:** [Documentar las opciones que se consideraron importantes]
- **Verificación:** [Cómo verificar que funciona]

*Es posible documentar múltiples métodos.*

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
1. **Descarga e instalación:**
- Visitar la página [dotnet](https://dotnet.microsoft.com/download).

![](screenshots/dotnet1.png)
- Descargar el SDK de .NET.

![](screenshots/dotnet2.png)
- Ejecutar el istalador y seguir el asistente.

![](screenshots/dotnet3.png)

1. **Verificación:** [Cómo comprobar que funciona]
- Abrir el terminal y ejecutar: `dotnet --version`
- Debe mostrar la versión del SDK instalada

![](screenshots/dotnet4.png)

### Configuración para C#

**Extensiones esenciales:**
- **C# Dev Kit** (Microsoft): Proporciona IntelliSense, debugging, navegación de código y gestión de proyectos.
- **C#** (Microsoft): Extensión base con soporte del lenguaje.

![](screenshots/dotnet5.png)

**Configuraciones específicas para C#:** 
- **Formateo automático al guardar**: Extensión Prettier - Code formatter

![](screenshots/dotnet6.png)
- **IntelliSense mejorado**: Se activa automáticamente con C# Dev Kit
- **Detección del SDK**: C# Dev Kit detecta automáticamente el SDK instalado
- **Auto-guardado**: File -> Auto Save

**Debugging básico:**
- **Breakpoints**: Click en el margen izquierdo del editor (aparece punto rojo)
- **Ejecutar y depurar**: Presionar F5 o icono "Run and Debug"
- **Inspección**: Variables visibles en panel lateral, hover para ver valores en tiempo real

![](screenshots/dotnet7.png)

> **Enfoque práctico**: El SDK .NET + VS Code te permite compilar, ejecutar y depurar sin necesidad de Visual Studio completo.

### Flujo de Trabajo con C#

**Creación de proyectos:**
[Documentar el proceso para crear proyectos C#]

**Estructura de proyecto:**

- En el siguiente código 
```csharp
string ShowMessage(string name)
{
    return $"Hola {name}, Bienvenido";
}

Console.WriteLine(ShowMessage(args.Length > 0 ? args[0] : "Nombre1"));
Console.WriteLine(ShowMessage(args.Length > 1 ? args[1] : "Nombre2"));
```

**Compilación y ejecución:**
Para compilar y ejecutar el código, sigue estos pasos:

1. **Compilación:**
   - Abre el terminal integrado en VS Code (Ctrl + `).
   - Navega hasta la carpeta del proyecto.
   - Ejecuta el siguiente comando para compilar el código:
     ```
     dotnet build
     ```

2. **Ejecución:**
   - Después de compilar, ejecuta el siguiente comando para ejecutar el código:
     ```
     dotnet run
     ```
- **Terminal integrado:** Uso del terminal dentro de VS Code para comandos `dotnet`

**Debugging:**
- **Breakpoints:** Cómo establecer y usar puntos de interrupción
- **Inspección de variables:** Uso del panel de variables y hover para ver valores en tiempo real
- **Control de ejecución:** Continuar (F5), Step Over (F10), Step Into (F11), Step Out (Shift+F11)
- **Call Stack:** Navegación por la pila de llamadas durante la depuración
- **Watch:** Añadir expresiones para monitorear su valor durante la depuración
- **Console:** Uso de la consola de depuración para evaluar expresiones y ver salidas
- **Configuración de launch.json:** Personalización de configuraciones de depuración si es necesario
---

## Visual Studio - IDE Alternativo

### Instalación

**Proceso de instalación:**
- **Descarga:** Visita la página oficial https://visualstudio.microsoft.com/es/
Se recomienda la versión Community (gratuita) o Professional (si se dispone de licencia).

![](screenshots/vs1.png)
- **Componentes necesarios:** Durante la instalación, selecciona la carga de trabajo:
Desarrollo de escritorio con .NET (incluye C#, Windows Forms, WPF, .NET SDK, y compiladores).

![](screenshots/vs2.png)
- **Verificación:** 
  - Abre Visual Studio.
  - Crea un nuevo proyecto C# (por ejemplo, “Consola .NET”).
  - Si el proyecto compila y ejecuta correctamente (“Hello World”), la instalación fue exitosa.
### Desarrollo con C#

**Creación de proyecto:**
[Describir el proceso para crear un proyecto C# en Visual Studio]

**Flujo de trabajo básico:**
- Compilación y ejecución
- Uso de Solution Explorer
- Debugging básico

---

## Configuración de Lenguaje Adicional

**Lenguaje seleccionado:** Python
**Justificación:** Python es un lenguaje versátil y fácil de aprender, ideal para desarrollo rápido y prototipado.

### Instalación del Entorno

**Runtime/SDK:**
- **Descarga e instalación:** Visitar la página oficial https://www.python.org/downloads/
- **Verificación:**
  - Abrir terminal y ejecutar: `python --version` o `python3 --version`
  - Debe mostrar la versión instalada

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

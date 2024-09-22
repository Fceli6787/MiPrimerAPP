# MiPrimerAPP
Desarrollado por Andres Felipe Celi Jimenez
Este repositorio contiene el código fuente de un proyecto desarrollado en Android utilizando **Jetpack Compose**, que implementa una interfaz gráfica con soporte para múltiples idiomas y ajustable a diferentes tamaños de pantalla. El proyecto está diseñado como una introducción a la creación de aplicaciones móviles modernas y escalables con una interfaz de usuario dinámica y responsiva.

## Características

1. **Soporte para múltiples idiomas**: 
   - La aplicación admite los siguientes idiomas:
     - Español (por defecto)
     - Inglés
     - Francés
     - Alemán
   - El idioma de la aplicación cambia automáticamente según la configuración regional del dispositivo.

2. **Diseño responsivo**:
   - La interfaz gráfica de usuario se adapta automáticamente a diferentes tamaños de pantalla y orientaciones, asegurando una experiencia consistente en dispositivos móviles de distintas resoluciones.
   - Se ha utilizado la imagen de fondo con el personaje de Android y una técnica de **Nine-patch** para mantener la proporción del gráfico sin deformaciones, independientemente de las dimensiones de la pantalla.

3. **Interfaz minimalista**:
   - La aplicación muestra un mensaje de bienvenida junto con un botón de "Entrar" en el centro de la pantalla.
   - El diseño está optimizado para proporcionar una experiencia visual limpia y sencilla, con un texto central grande y un botón accesible para los usuarios.

4. **Uso de tecnologías modernas**:
   - Implementación de **Jetpack Compose**, el nuevo kit de herramientas para construir interfaces de usuario en Android de manera declarativa.
   - Arquitectura simple, pero extensible, basada en la actividad principal de Android y componentes de UI reutilizables.

## Requisitos del Sistema

- **Android Studio**: Versión 4.2 o superior.
- **Gradle**: Compatible con versiones 7.0 o superiores.
- **SDK**: API 21 o superior.
- **Emulador o dispositivo físico** con Android 5.0 (Lollipop) o superior.

## Instalación

1. Clona el repositorio en tu máquina local:

   ```bash
   git clone https://github.com/usuario/mi-primera-app-android.git
   ```

2. Abre el proyecto en **Android Studio**.

3. Conecta un emulador o un dispositivo físico y ejecuta la aplicación mediante el botón `Run`.

4. La aplicación se instalará y se ejecutará en el dispositivo/emulador.

## Estructura del Proyecto

- **MainActivity.kt**: El archivo principal donde se gestiona la lógica y el ciclo de vida de la actividad.
- **Composables**: Se han definido funciones `@Composable` para crear la interfaz de usuario de forma modular y reutilizable.
- **res/values/strings.xml**: Contiene los recursos de texto localizados para los cuatro idiomas soportados.
- **res/drawable/marcianito_background.9.png**: Imagen de fondo en formato nine-patch, utilizada para mantener la correcta proporción del gráfico de Android en todas las resoluciones de pantalla.

## Uso del Archivo Nine-Patch

Para lograr un fondo que no distorsione el personaje de Android al redimensionar la ventana, se ha utilizado un archivo **nine-patch**. Esta técnica permite que ciertas partes de la imagen se estiren mientras otras permanecen estáticas. El archivo `marcianito_background.9.png` se ha creado utilizando la herramienta **Draw 9-patch** de Android Studio.

## Localización (Multilenguaje)

El archivo `strings.xml` se ha modificado para incluir traducciones para los cuatro idiomas mencionados. El cambio de idioma en la aplicación se gestiona automáticamente a través de la configuración del sistema operativo del dispositivo. A continuación se muestran ejemplos de los recursos utilizados:

### Español (predeterminado)
```xml
<resources>
    <string name="app_name">Mi Primera App</string>
    <string name="greeting_message">Hola %1$s!</string>
</resources>
```

### Inglés
```xml
<resources>
    <string name="app_name">My First App</string>
    <string name="greeting_message">Hello %1$s!</string>
</resources>
```

### Francés
```xml
<resources>
    <string name="app_name">Mon Première Application</string>
    <string name="greeting_message">Bonjour %1$s!</string>
</resources>
```

### Alemán
```xml
<resources>
    <string name="app_name">Meine Erste App</string>
    <string name="greeting_message">Hallo %1$s!</string>
</resources>
```

## Compatibilidad con múltiples pantallas

Se ha implementado el soporte para múltiples tamaños de pantalla mediante el uso de **modificadores** en Jetpack Compose y la optimización del diseño utilizando principios de diseño responsivo. Esto garantiza que la aplicación se vea bien en dispositivos pequeños y grandes, tanto en orientación vertical como horizontal.

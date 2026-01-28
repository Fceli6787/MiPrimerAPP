# MiPrimerAPP

[![Android](https://img.shields.io/badge/Android-5.0%2B-brightgreen)](https://www.android.com/)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-Latest-blue)](https://developer.android.com/jetpack/compose)
[![Kotlin](https://img.shields.io/badge/Kotlin-1.8%2B-purple)](https://kotlinlang.org/)

Una aplicación móvil moderna desarrollada en Android con **Jetpack Compose** que demuestra conceptos fundamentales de desarrollo Android, incluyendo soporte multiidioma, diseño responsivo y arquitectura escalable.

**Desarrollado por:** Andres Felipe Celi Jimenez

---

## 📋 Características Principales

### 🌍 Soporte Multiidioma
La aplicación soporta **4 idiomas** con cambio automático según la configuración del dispositivo:
- 🇪🇸 **Español** (por defecto)
- 🇬🇧 **Inglés**
- 🇫🇷 **Francés**
- 🇩🇪 **Alemán**

### 📱 Diseño Responsivo
- Interfaz adaptativa que se ajusta automáticamente a diferentes tamaños de pantalla
- Compatible con orientación vertical y horizontal
- Imagen de fondo con técnica Nine-patch para evitar distorsiones
- Experiencia consistente en dispositivos de todas las resoluciones

### ✨ Interfaz Minimalista
- Diseño limpio y moderno con Jetpack Compose
- Mensaje de bienvenida personalizado
- Botón de navegación intuitivo
- Enfoque en la experiencia del usuario

### 🏗️ Arquitectura Moderna
- Implementación completa con **Jetpack Compose**
- Componentes UI reutilizables y modulares
- Código limpio y mantenible
- Base extensible para futuros desarrollos

---

## 🚀 Requisitos del Sistema

| Requisito | Versión Mínima |
|-----------|-----------------|
| Android Studio | 4.2 o superior |
| Gradle | 7.0 o superior |
| SDK de Android | API 21+ |
| Runtime Android | 5.0 (Lollipop) o superior |
| Lenguaje | Kotlin 1.8+ |

---

## 📦 Instalación

### Paso 1: Clonar el repositorio
```bash
git clone https://github.com/usuario/mi-primera-app-android.git
cd mi-primera-app-android
```

### Paso 2: Abrir en Android Studio
1. Abre Android Studio
2. Selecciona **File** → **Open** (Archivo → Abrir)
3. Navega a la carpeta clonada y selecciona el proyecto

### Paso 3: Ejecutar la aplicación
1. Conecta un dispositivo físico o inicia un emulador
2. Haz clic en el botón **Run** (▶) o presiona `Shift + F10`
3. Selecciona el dispositivo/emulador destino
4. ¡La aplicación se instalará y ejecutará automáticamente!

---

## 📁 Estructura del Proyecto

```
mi-primera-app-android/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/
│   │   │   │   └── MainActivity.kt          # Actividad principal
│   │   │   ├── res/
│   │   │   │   ├── values/
│   │   │   │   │   └── strings.xml         # Recursos localizados (Español)
│   │   │   │   ├── values-en/
│   │   │   │   │   └── strings.xml         # Traducción Inglés
│   │   │   │   ├── values-fr/
│   │   │   │   │   └── strings.xml         # Traducción Francés
│   │   │   │   ├── values-de/
│   │   │   │   │   └── strings.xml         # Traducción Alemán
│   │   │   │   ├── drawable/
│   │   │   │   │   └── marcianito_background.9.png  # Imagen Nine-patch
│   │   │   │   └── layout/
│   │   │   └── AndroidManifest.xml
│   │   └── test/
│   ├── build.gradle.kts
│   └── proguard-rules.pro
├── build.gradle.kts
├── settings.gradle.kts
└── README.md
```

---

## 🎯 Descripción de Componentes Clave

### MainActivity.kt
Actividad principal de la aplicación que gestiona:
- Ciclo de vida de la aplicación
- Lógica de la interfaz de usuario
- Integración con Jetpack Compose

### Composables
Funciones `@Composable` que definen:
- Componentes UI reutilizables
- Layout responsivo
- Manejo de estados

### Localización (strings.xml)
Archivos de recursos en múltiples idiomas para soporte multiidioma automático:

**Español (es-ES):**
```xml
<string name="app_name">Mi Primera App</string>
<string name="greeting_message">¡Hola %1$s!</string>
<string name="enter_button">Entrar</string>
```

**Inglés (en):**
```xml
<string name="app_name">My First App</string>
<string name="greeting_message">Hello %1$s!</string>
<string name="enter_button">Enter</string>
```

**Francés (fr):**
```xml
<string name="app_name">Ma Première Application</string>
<string name="greeting_message">Bonjour %1$s!</string>
<string name="enter_button">Entrer</string>
```

**Alemán (de):**
```xml
<string name="app_name">Meine Erste App</string>
<string name="greeting_message">Hallo %1$s!</string>
<string name="enter_button">Betreten</string>
```

### Imagen de Fondo Nine-Patch
El archivo `marcianito_background.9.png` utiliza la técnica Nine-patch para:
- Evitar distorsiones del personaje de Android
- Mantener proporciones correctas en todas las resoluciones
- Escalar solo las áreas especificadas

**Creación:** Herramienta Draw 9-patch en Android Studio

---

## 💡 Conceptos Implementados

✅ **Jetpack Compose** - Framework moderno para UI declarativa  
✅ **Kotlin** - Lenguaje de programación moderno y seguro  
✅ **Localización** - Soporte multiidioma automático  
✅ **Diseño Responsivo** - Adaptación a múltiples pantallas  
✅ **Recursos Android** - Gestión eficiente de assets  
✅ **Nine-patch Images** - Escalado inteligente de gráficos  
✅ **Arquitectura Modular** - Componentes reutilizables  

---

## 🔧 Configuración del Proyecto

### Gradle (build.gradle.kts)
```kotlin
android {
    compileSdk = 34
    
    defaultConfig {
        minSdk = 21
        targetSdk = 34
    }
    
    buildFeatures {
        compose = true
    }
}

dependencies {
    implementation("androidx.compose.ui:ui")
    implementation("androidx.compose.material3:material3")
    // ... otras dependencias
}
```

---

## 🎓 Casos de Uso Educativos

Esta aplicación es ideal para aprender:
- Fundamentos de desarrollo Android moderno
- Uso de Jetpack Compose para UI declarativa
- Implementación de multiidioma en aplicaciones
- Diseño responsivo y adaptativo
- Buenas prácticas de arquitectura Android
- Gestión de recursos en Android Studio

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Para contribuir:

1. Haz un fork del proyecto
2. Crea una rama para tu característica (`git checkout -b feature/MiCaracteristica`)
3. Commitea tus cambios (`git commit -m 'Agrego: Descripción de la característica'`)
4. Haz push a la rama (`git push origin feature/MiCaracteristica`)
5. Abre un Pull Request

---

## 📄 Licencia

Este proyecto está disponible bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.

---

## 👨‍💻 Autor

**Andres Felipe Celi Jimenez**
---

## 📚 Recursos Útiles

- [Documentación Jetpack Compose](https://developer.android.com/jetpack/compose)
- [Android Developers](https://developer.android.com/)
- [Kotlin Documentation](https://kotlinlang.org/docs/)
- [Android Material Design](https://material.io/design)
- [Nine-patch in Android](https://developer.android.com/guide/topics/graphics/2d-graphics#nine-patch)

---

## 🐛 Problemas y Soporte

Si encuentras algún problema o tienes sugerencias:

1. Abre un [Issue](https://github.com/usuario/mi-primera-app-android/issues)
2. Describe el problema detalladamente
3. Incluye capturas de pantalla si es relevante
4. Especifica tu versión de Android y dispositivo

---

## ⭐ Si te fue útil

¡No olvides dejar una estrella ⭐ si este proyecto te ayudó!

---

**Última actualización:** Enero 2026

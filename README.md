<div align="center">

# SwiftUI Sign Up

**Prototipo de una pantalla de registro para iOS, desarrollado con SwiftUI y enfocado en una experiencia visual moderna.**

![Swift](https://img.shields.io/badge/Swift-5.0-F05138?logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-iOS-0D96F6?logo=swift&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-15.4%2B-000000?logo=apple&logoColor=white)
![Estado](https://img.shields.io/badge/estado-prototipo-8B5CF6)

</div>

## Descripción

SwiftUI Sign Up es una demostración de interfaz para una pantalla de creación de cuenta. El diseño combina fondos ilustrados, transparencias, desenfoque, campos personalizados y gradientes para construir una experiencia atractiva y reutilizable.

> Este proyecto demuestra la interfaz y sus interacciones visuales. No incluye un servicio de autenticación ni conexión con un backend.

## Vista previa

<div align="center">
  <img src="https://user-images.githubusercontent.com/20882895/192369100-2d6e107b-7117-4ce6-8184-ac0c93c245d6.png" alt="Pantalla de registro" width="300">
  &nbsp;&nbsp;
  <img src="https://user-images.githubusercontent.com/20882895/192369111-eb96af37-c419-47b3-a152-2b54aaf88292.png" alt="Interacción con el formulario" width="300">
</div>

## Características

- Formulario de registro con correo electrónico y contraseña.
- Campos personalizados con indicadores visuales de foco.
- Botón y textos con gradientes.
- Efecto de cristal mediante desenfoque y transparencias.
- Diseño adaptable construido con componentes de SwiftUI.
- Recursos visuales organizados en un catálogo de assets.

## Tecnologías

- **Swift 5**
- **SwiftUI**
- **UIKit** para el efecto visual y el selector de imágenes
- **Core Data**
- **Xcode**

## Estructura

```text
Presentacion/
├── Shared/     # Aplicación, vista principal, persistencia y recursos
├── Views/      # Componentes visuales reutilizables
├── Helpers/    # Desenfoque y selector de imágenes
├── macOS/      # Configuración del target de macOS
└── Presentacion.xcodeproj
```

## Requisitos

- macOS con Xcode
- iOS 15.4 o posterior
- Swift 5.0 o posterior

## Instalación

1. Cloná el repositorio:

   ```bash
   git clone https://github.com/luchonicolini/Presentacion.git
   ```

2. Abrí el proyecto:

   ```bash
   open Presentacion/Presentacion.xcodeproj
   ```

3. Seleccioná el target de iOS y un simulador compatible.
4. Ejecutá la aplicación con `⌘R`.

## Autor

Desarrollado por [Luciano Nicolini](https://github.com/luchonicolini).

Si te resulta útil como referencia de diseño en SwiftUI, podés dejar una ⭐ en el repositorio.

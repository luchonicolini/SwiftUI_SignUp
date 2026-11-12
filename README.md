# SwiftUI Sign Up

> **English:** An iOS sign-up UI prototype exploring reusable SwiftUI components, custom focus feedback, gradients and translucent surfaces. It demonstrates interface composition, not a working authentication backend.

Este prototipo explora cómo construir un formulario de registro con una identidad visual propia y componentes reutilizables.
Permite revisar la composición, el foco de los campos y los estados visuales de email y contraseña.

**Alcance:** demostración de UI. Los botones no crean cuentas ni inician sesión.

## Capturas

<img src="https://user-images.githubusercontent.com/20882895/192369100-2d6e107b-7117-4ce6-8184-ac0c93c245d6.png" alt="Formulario de registro con superficie translúcida" width="300">
<img src="https://user-images.githubusercontent.com/20882895/192369111-eb96af37-c419-47b3-a152-2b54aaf88292.png" alt="Estado visual del formulario de registro" width="300">

## Funcionalidades

- Campos de email y contraseña con estado local.
- Indicadores visuales del campo en edición.
- Botón y texto con gradientes, separados en componentes.
- Superficies translúcidas con un adaptador de desenfoque UIKit.
- Recursos gráficos y colores centralizados en el catálogo de assets.

## Stack y estructura

| Área | Implementación |
| --- | --- |
| Lenguaje y UI | Swift 5 y SwiftUI |
| Destino iOS | iOS 15.4 o posterior, según el proyecto |
| Estado | `@State` en la vista; no hay una capa MVVM de autenticación |
| Interoperabilidad | UIKit en helpers de interfaz |
| Persistencia | Infraestructura Core Data de la plantilla; no guarda registros de usuarios |

| Ubicación | Responsabilidad |
| --- | --- |
| `Shared/ContentView.swift` | Composición del formulario |
| `Views/` | GradientButton, GradientText y TextfieldIcon |
| `Helpers/` | Desenfoque y selector de imágenes |
| `Shared/Assets.xcassets/` | Imágenes y colores |
| `Shared/Persistence.swift` | Infraestructura de persistencia de la plantilla |

## Cómo ejecutarlo

1. Instalá Xcode en macOS y un simulador compatible.
2. Cloná y abrí el proyecto desde la raíz:

   ```bash
   git clone https://github.com/luchonicolini/SwiftUI_SignUp.git
   cd SwiftUI_SignUp
   open Presentacion.xcodeproj
   ```

3. Seleccioná el target/esquema de **Presentacion (iOS)** y un simulador con iOS 15.4 o posterior.
4. Compilá y ejecutá con **⌘R**.
5. Para un dispositivo físico, configurá tu propio equipo de firma.

El proyecto incluye configuración macOS heredada. El alcance documentado aquí es el prototipo iOS.

## Verificación

Revisá manualmente entrada de texto, foco, teclado y comportamiento en distintos tamaños de pantalla.
El repositorio no tiene suite automatizada ni workflow de CI.
Las capturas conservadas sirven como referencia visual; no certifican compatibilidad con versiones nuevas de iOS.

## Próximos pasos

- Validar contraste, tamaños de texto, VoiceOver y navegación por teclado.
- Agregar validaciones y estados de carga y error si se convierte en un flujo real.
- Incorporar pruebas de interacción antes de integrar un proveedor de autenticación.
- Documentar el origen de los recursos y las referencias visuales.

## Pendientes de presentación

- [COMPLETAR: referencias del ejercicio y atribución o licencia de los recursos visuales]

## Autor

[Luciano Nicolini](https://github.com/luchonicolini) · iOS Developer (Swift, SwiftUI).

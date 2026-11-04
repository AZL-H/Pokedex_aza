# 📱💻 Pokédex App (Flutter Cross-Platform)

Una aplicación de Pokédex moderna y robusta desarrollada en **Flutter**, diseñada para ofrecer una experiencia nativa fluida tanto en dispositivos móviles (**Android**) como en navegadores web (**Google Chrome**) gracias a su arquitectura híbrida con persistencia local mediante **SQLite** y **WebAssembly (IndexedDB)**.

---

## ✨ Características Principales

### 🔍 Catálogo y Búsqueda Avanzada
* **Paginación Fluida:** Carga optimizada mediante *infinite scroll* con filtros de duplicados para evitar condiciones de carrera.
* **Búsqueda Instantánea:** Barra de búsqueda con sistema de *Debounce* para consultar Pokémon por nombre o número de Pokedex de forma eficiente.
* **Filtros Dinámicos:** Sistema de filtrado por **Tipo** y **Generación** mediante chips interactivos y botón de reseteo rápido.

### 🛡️ Gestión y Creación de Equipos (Rúbrica Escolar)
* **CRUD Completo:** Crear, nombrar, editar y eliminar equipos personalizados.
* **Regla de Negocio Estricta:** Límite máximo de **6 Pokémon por equipo**, con validación en base de datos y alertas visuales instantáneas mediante `SnackBar`.
* **Persistencia Local Relacional:** Almacenamiento local mediante SQLite, integrando claves foráneas con borrado en cascada (`ON DELETE CASCADE`).
* **Resumen de Integrantes:** Visualización rápida de los miembros del equipo con opciones de retiro y análisis táctico.

### 🌟 Detalle y Experiencia de Usuario
* **Vista de Detalles Enriquecida:** Estadísticas base con barras de progreso animadas, tipos elementales, peso, altura y habilidades.
* **Toggle Shiny & Cries:** Alterna dinámicamente entre el sprite normal y la versión variocolor (*Shiny*), y reproduce los gritos oficiales de los Pokémon mediante `audioplayers`.
* **Cadena Evolutiva:** Navegación interactiva entre las diferentes etapas de evolución de cada criatura.
* **Sistema de Favoritos:** Guarda y gestiona tus Pokémon favoritos con persistencia local.

---

## 🛠️ Stack Tecnológico y Arquitectura

* **Framework:** Flutter & Dart
* **Tipografía y Estilos:** `Google Fonts` (Poppins y Nunito) y diseño basado en Material Design adaptado.
* **Base de Datos (Multiplataforma):**
  * **Móvil (Android):** `sqflite` con rutas nativas del dispositivo.
  * **Web (Chrome):** `sqflite_common_ffi_web` operando sobre WebAssembly (**WASM**) e `IndexedDB`.
* **Consumo de APIs:** Conexión directa a la **PokéAPI** oficial para obtención de datos y sprites oficiales de alta resolución.
* **Multimedia:** `cached_network_image` (con renderizado adaptable a `Image.network` para garantizar estabilidad absoluta en Flutter Web) y `audioplayers`.

---

## 🚀 Cómo Ejecutar el Proyecto

Sigue estos pasos para clonar y ejecutar la aplicación en tu entorno local:

1. **Clona el repositorio:**
   ```bash
   git clone [https://github.com/AZL-H/Pokedex_aza]([https://github.com/tu-usuario/pokedex_app.git](https://github.com/AZL-H/Pokedex_aza)

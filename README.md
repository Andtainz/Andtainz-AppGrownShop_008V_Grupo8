
# 📱 Proyecto Móvil – Gestión de Aplicación

**Autor:** Joshua Mardonez

## 🚀 Descripción

Este proyecto corresponde a una aplicación móvil desarrollada como parte de un taller académico.
El objetivo principal es implementar un flujo de navegación que permita al usuario:

* Autenticarse en el sistema (login/registro).
* Acceder a un conjunto de funcionalidades principales.
* Consumir y gestionar datos mediante APIs.
* Explorar pantallas secundarias que dependen de la información principal.

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Kotlin / Java (Android)
* **Arquitectura:** MVC / MVVM (dependiendo de la implementación observada en `src/`)
* **Backend:** API REST (endpoints consumidos para persistencia de datos)
* **Base de datos:** SQLite / API remota (según configuración del proyecto)
* **Entorno de desarrollo:** Android Studio

## 📂 Estructura del Proyecto

```
Proyecto_Movil/
│── src/                # Código fuente principal
│   ├── activities/     # Pantallas (UI y lógica de interacción)
│   ├── fragments/      # Vistas reutilizables
│   ├── models/         # Modelos de datos
│   ├── adapters/       # Adaptadores (RecyclerView, listas, etc.)
│   ├── api/            # Conexión con servicios externos
│   └── utils/          # Funciones auxiliares y helpers
│
│── res/                # Recursos gráficos (layouts, drawables, values)
│── manifest/           # Configuración principal de la app
│── gradle/             # Configuración de dependencias
```

## 🔄 Flujo de la Aplicación

1. **Inicio de la app**

   * El usuario abre la aplicación y se muestra la pantalla de *login/registro*.

2. **Autenticación**

   * Se valida al usuario contra la base de datos / API.
   * Si es correcto → acceso a la pantalla principal.
   * Si falla → mensaje de error.

3. **Pantalla principal (Home / Dashboard)**

   * Aquí se centralizan las funciones principales (ej. catálogo, usuarios, pedidos, etc.).

4. **Consumo de API / Base de Datos**

   * Las entidades (productos, usuarios, pedidos) se obtienen mediante llamadas a servicios REST.
   * Se procesan y renderizan en la UI (ej: listas con RecyclerView).

5. **Pantallas secundarias**

   * Acciones específicas como crear, editar o eliminar registros.
   * Ejemplo: crear pedido, ver detalles de producto, editar perfil.

6. **Cierre de sesión**

   * El usuario puede cerrar sesión y volver al *login*.

## 📌 Características Clave

* Navegación dinámica entre pantallas.
* Manejo de usuarios y autenticación.
* Consumo de APIs REST.
* Persistencia local y/o remota de datos.
* Diseño modular y escalable.

## ⚙️ Instalación y Ejecución

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/usuario/proyecto-movil.git
   ```
2. Abrir el proyecto en **Android Studio**.
3. Sincronizar dependencias Gradle.
4. Ejecutar en un emulador o dispositivo físico.

## 👨‍💻 Autor

**Joshua Mardonez** – Proyecto académico de aplicación móvil.

---

👉 ¿Quieres que te arme también un **diagrama visual del flujo** (en Mermaid o imagen) para complementar el README y que se entienda mejor el recorrido del usuario?

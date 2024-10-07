# Taller2
 
Link al repositorio: https://github.com/siraglez/Taller2.git

Esta aplicación de Android permite a los usuarios gestionar su nombre y seleccionar un color de fondo para la interfaz. La aplicación está desarrollada utilizando Jetpack Compose y utiliza `SharedPreferences` para almacenar el nombre y el color seleccionado.

## Estructura de la Aplicación

La aplicación consta de tres pantallas principales:

1. **Pantalla de Bienvenida (`MainActivity`)**
   - Muestra un saludo personalizado según la hora del día (buenos días, buenas tardes o buenas noches).
   - Incluye un botón para navegar a la **Actividad Principal**.

2. **Actividad Principal (`ActividadPrincipal`)**
   - Permite al usuario ingresar y guardar su nombre. El nombre se almacena en `SharedPreferences`.
   - Muestra el nombre ingresado después de guardarlo.
   - Incluye un botón que navega a la **Pantalla de Configuración**.
   - Proporciona un botón para iniciar una tarea en segundo plano que simula una operación de red y muestra el progreso de esta tarea utilizando un `CircularProgressIndicator`. El progreso se actualiza y muestra en tiempo real.

3. **Pantalla de Configuración (`PantallaConfiguracion`)**
   - Permite al usuario seleccionar un color de fondo de la aplicación.
   - Incluye botones para elegir entre varios colores (Rojo, Azul, Verde, y Gris Claro).
   - Al seleccionar un color, se guarda en `SharedPreferences`, y la aplicación cambia su color de fondo a la selección del usuario.
   - Un botón de retorno permite volver a la pantalla de bienvenida.

## Funcionalidades Principales

- **Gestión de Nombre**: Los usuarios pueden ingresar y guardar su nombre, que se mostrará en la interfaz.
- **Selección de Color**: La aplicación permite a los usuarios personalizar el color de fondo, el cual se guarda para sesiones futuras.
- **Tarea en Segundo Plano**: Se simula una operación de red utilizando `AsyncTask`, que actualiza el progreso en tiempo real.

## Tecnologías Utilizadas

- **Android SDK**: Para el desarrollo de la aplicación.
- **Jetpack Compose**: Para construir la interfaz de usuario.
- **SharedPreferences**: Para almacenar datos persistentes como el nombre del usuario y el color de fondo.
- **AsyncTask**: Para manejar tareas en segundo plano que simulan operaciones de red.

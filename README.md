# Demostración tecnológica de Svelte para la Proof Of Concept | DSW 2024

Esta demostración tecnológica fue desarrollada para la exposición de la materia **Desarrollo de Software**. El propósito del proyecto es exhibir las funcionalidades y capacidades del framework **Svelte**, mediante el desarrollo de una web similar a la página de la UTN Rosario pero con funciones más limitadas.

## Descripción

El proyecto consiste en una página web demostrativa que busca replicar la estructura básica de la web de la facultad. Los principales objetivos de esta demostración son:

- Mostrar cómo se pueden utilizar componentes en Svelte.
- Implementar una estructura modularizada que facilite la escalabilidad.
- Demostrar cómo se gestionan los datos estáticos y dinámicos.

### Funcionalidades

- **Acceso al CVG:** Una sección con acceso directo al sistema de gestión de contenidos de la facultad.
- **Acceso al SYSACAD:** Un acceso directo al Sistema de Autogestión de Alumnos.
- **Información de tecnicaturas:** Un apartado de información que muestre las tecnicaturas ofrecidas por la facultad.

- **Noticias e imagenes institucionales:** Se exponen distintas noticias propias de la universidad y un carrousel de imagenes para mostrar aquellas destacadas.

- **Horarios de atención:** Una sección información que cuenta con la descripción de los horarios de atención para alumnos y egresados, la dirección en forma de mapa de la facultad y un formulario para enviar una consulta.

## Estructura del Proyecto

El proyecto está compuesto por las siguientes rutas:

- **/institucional:** Se muestra un carrousel con imagenes demostrativas y pequeñas descripciones de las mismas. Le siguen un apartado de noticias traidas desde `news.json`

- **/informacion:** La cual muestra los accesos a las páginas de autogestión, los horarios de contacto traídos desde `horarios.json` y un formulario de contacto.

- **/tecnicaturas:** Donde se muestran cards con algunas de las tecnicaturas brindadas por la Universidad.

- **/desarrollo:** Se muestra el componente `desarrollo.svelte` el cual utilizamos para acortar las funcionalidades de la página.

### Archivo principal

- `+page.svelte`: Página principal que organiza los componentes y muestra la estructura completa de la web.

## Tecnologías utilizadas

- **Svelte:** Framework principal del proyecto para construir interfaces de usuario reactivas.
- **Vite:** Herramienta para el build y desarrollo de la aplicación.

## Instalación

Para ejecutar este proyecto localmente, sigue estos pasos:

1. Clona este repositorio.
2. Instala las dependencias con el siguiente comando:

   ```bash
   npm install

Ejecuta el servidor de desarrollo:

    npm run dev

Abre tu navegador en <http://localhost:5173> para ver el proyecto en acción.

## Autores

El grupo de **Svelte** en la categoría de **frontend-frameworks** fue integrado por:

- Boggio Valentino.
- Larrauri Martina.
- Leali Bruno.
- Zapata Nicolás.

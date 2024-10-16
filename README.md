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
- **Información de carreras:** Un apartado de información que muestre las carreras ofrecidas por la facultad, indicando descripciones, perfiles del ingeniero, títulos intermedios, planes de estudio, etc.

## Estructura del Proyecto

El proyecto está compuesto por los siguientes componentes:

- `Header.svelte`: Encabezado de la página con navegación a las secciones principales.
- `WelcomeSection.svelte`: Sección de bienvenida con un mensaje personalizado de acuerdo a la URL donde se encuentra.
- `CardGrid.svelte`: Contenedor de las tarjetas para organizar la presentación visual.
- `Card.svelte`: Componente individual de tarjeta para mostrar accesos a distintos apartados.
- `Footer.svelte`: Pie de página con información institucional y del grupo.

### Archivos principales

- `data.json`: Archivo de datos que contiene información estática sobre las carreras.
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

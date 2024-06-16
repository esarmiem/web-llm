#Web LLM's

## Descripción

Este proyecto ofrece una implementación local de ollama, permitiendo a los usuarios interactuar con un modelo de lenguaje avanzado directamente desde su navegador sin necesidad de conexión a internet. La aplicación está diseñada para ser completamente privada y gratuita, proporcionando una experiencia de chat intuitiva y eficiente.

## Características Principales

- **Privacidad**: Todas las interacciones son procesadas localmente, garantizando la seguridad y confidencialidad de los datos.
- **Acceso Gratuito**: No hay costos asociados con el uso de esta herramienta.
- **Interfaz Intuitiva**: Una interfaz amigable que facilita la comunicación con el modelo de lenguaje.
- **Modelo Avanzado**: Utiliza el modelo Llama-3-8B-Instruct-q4f32_1-MLC-1k para generar respuestas precisas y relevantes.

## Requisitos

Para utilizar esta aplicación, asegúrate de tener acceso a un navegador moderno compatible con Web Workers y módulos ES.

## Uso

1. Abre el archivo HTML en tu navegador.
2. Espera a que se cargue el modelo de lenguaje. Esto puede tomar un tiempo, dependiendo de la potencia de tu dispositivo y tu conexión a internet.
3. Verás un campo de entrada donde puedes escribir tus mensajes.
4. Haz clic en el botón "Enviar" para enviar tu mensaje al modelo.
5. Recibirás respuestas instantáneas del modelo de lenguaje.

## Código Fuente

El código fuente incluye tanto el frontend como el backend necesario para ejecutar la aplicación:

### Frontend (`index.html`)

El archivo `index.html` contiene todo el código necesario para la interfaz de usuario y la interacción con el modelo de lenguaje. Utiliza CSS para estilizar la aplicación y JavaScript para manejar la lógica de la aplicación, incluyendo la comunicación con el modelo de lenguaje a través de un Web Worker.

### Backend (`worker.js`)

El archivo `worker.js` actúa como un Web Worker que comunica con el modelo de lenguaje utilizando la biblioteca `@mlc-ai/web-llm`. Este archivo es responsable de recibir mensajes del frontend, procesarlos mediante el modelo de lenguaje y devolver las respuestas al frontend.

## Contribuciones

Las contribuciones son bienvenidas. Si tienes ideas para mejorar esta aplicación o encuentras algún error, por favor abre un issue o haz un pull request.

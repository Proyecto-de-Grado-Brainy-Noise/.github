![logo-no-background](https://github.com/Proyecto-de-Grado-Brainy-Noise/.github/assets/78034097/2da46487-16de-45d4-a66d-14f4f95f0581)

# Integrantes:
 - Estefanía Bermúdez Arroyo
 - Jessica Tatiana Naizaque Guevara 
 - Juan Sebastián Vargas Torres 

# Descripción general:

Es un prototipo web que permite cargar resonancias magnéticas del cerebro humano y mediante el uso de un modelo de aprendizaje de máquina, obtiene una respuesta con la identificación del nivel de ruido (presencia o ausencia) de las imágenes. 

![arq_alto_nivel](https://github.com/Proyecto-de-Grado-Brainy-Noise/.github/assets/78034097/0a5e71b0-e366-4ed5-9801-b24701794fd3)

## Frontend:

Este componente es el encargado de la creación de la interfaz gráfica con la cual el usuario va a interactuar. Este usa Angular como framework y realiza llamados HTTP al API Gatway del sistema. A continuación, mediante el siguiente link se puede acceder al repositorio: [Frontend repo](https://github.com/Proyecto-de-Grado-Brainy-Noise/Frontend).

<p align="center">
  <img src="https://github.com/Proyecto-de-Grado-Brainy-Noise/.github/assets/78034097/8a7fe392-81ba-401a-9914-1988e2fcc359" width="400" height="500" />
</p>

## Gestión de Usuarios:

Este componente es el encargado de manegar el CRUD de usuarios que puede realizar el usuario con rol de administrador. Este usa Spring Boot como framework y se conecta a la base datos mediante JPA. A continuación, por medio del siguiente link se puede acceder al repositorio: [user_management](https://github.com/Proyecto-de-Grado-Brainy-Noise/user_management).

## Modelo:

Este componente es el encargado de recibir la resonancia y su información asociada y posterior a esto generar la predicción de nivel de ruido junto con la confianza de esta. Este usa Django como framework, RabbitMQ como broker, Celery como encolador de tareas y MongoDB para el manejo de base de datos no relacional. A continuación, por medio del siguiente link se puede acceder al repositorio: [ModelService](https://github.com/Proyecto-de-Grado-Brainy-Noise/modelService).

<img width="1242" alt="arquitecturaodelo" src="https://github.com/Proyecto-de-Grado-Brainy-Noise/.github/assets/78034097/f2e4ce86-0e33-4ff1-9637-203f26258b6e">

## Consulta:

Este componte se encarga que realizar consultas sobre la base de datos no relacional acerca de los resultados obtenidos de las predicciones realizadas, ofreciendo consultas tanto para obtener los datos en el response o como un archivo CSV, esto tanto para una sola predicción como de todo el historial de predicciones asociadas a un email. A continuación, por medio del siguiente link se puede acceder al repositorio: [queryResultsService](https://github.com/Proyecto-de-Grado-Brainy-Noise/queryResultsService).

## API Gateway: 

Este componenete es el encargado de recibir todas la peticiones HTTP realizadas desde el frontend y redirigirlas a los microservicios solicitados. Este usa Spring Boot como framework. A continuación, por medio del siguiente link se puede acceder al repositorio: [queryResultsService](https://github.com/Proyecto-de-Grado-Brainy-Noise/api_gateway).

## Docker Compose:

Este archivo nos permite correr todo el proyecto, esto incluye:

- Frontend
- API Gateway
- Microservicios (Gestión de usuario, Modelo, Consultas)
- Bases de datos relacional y no relacional
- Red de Docker
- Volúmenes necesarios}

A continuación, por medio del siguiente link se puede acceder al repositorio: [queryResultsService](https://github.com/Proyecto-de-Grado-Brainy-Noise/docker-compose).
<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

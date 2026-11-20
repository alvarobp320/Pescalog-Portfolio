# PescaLog

> **Una app móvil para registrar y gestionar capturas de pesca, generar estadísticas, añadir y competir contra amigos.**

PescaLog es un proyecto personal en desarrollo que explora cómo llevar la experiencia de pesca al móvil: reunir y gestionar la información de cada jornada, generar estadísticas, competir contra amigos y mucho más.

Este repositorio presenta el proyecto desde el punto de vista del producto. Aquí encontrarás su propósito, la arquitectura prevista, las tecnologías y el estado actual, sin código de la aplicación.

## El proyecto en un vistazo

| | |
|---|---|
| **Tipo** | Aplicación móvil |
| **Plataformas objetivo** | Android e iOS |
| **Cliente móvil** | React Native con Expo |
| **Backend** | Java |
| **Persistencia** | PostgreSQL |
| **Estado** | Desarrollo; todavía sin despliegue público |

## La idea

Las jornadas de pesca generan recuerdos que pueden quedar dispersos. PescaLog busca ofrecer un lugar práctico desde el que registrar y consultar esa actividad, así como comprobar nuestras estadísticas y competir contra amigos, con una experiencia móvil sencilla y una arquitectura cliente-servidor que permita evolucionar el producto.

El alcance funcional continúa en construcción. Este portfolio evita presentar como terminadas funciones que todavía no han sido verificadas como parte de una versión publicada. Ha sido probado en emuladores de Android e iOS, con éxito.

## Tecnologías

- **React Native** para la experiencia móvil multiplataforma.
- **Expo** para el entorno de desarrollo y la gestión de la aplicación.
- **Expo Router** para la navegación de la app.
- **Java** para los servicios del backend.
- **PostgreSQL** como base de datos relacional.
- **JWT** como mecanismo previsto para autenticar las peticiones.
- **Expo SecureStore** disponible en el cliente para almacenamiento seguro de credenciales o sesión.

Consulta [Tecnologías y arquitectura](docs/tecnologias-y-arquitectura.md) para conocer cómo encajan las piezas y qué partes siguen pendientes.

## Estado actual

- La app móvil se ha iniciado en entorno Android con Expo.
- La estructura contempla un cliente React Native, una API Java y PostgreSQL.
- La autenticación con JWT forma parte del flujo planteado.
- El backend, la base de datos y la app aún no están desplegados públicamente.
- No hay publicación disponible en App Store ni Google Play.

El detalle y los siguientes pasos están en [Estado y hoja de ruta](docs/estado-y-hoja-de-ruta.md).

## Recorrido de la presentación

- [Visión del producto](docs/vision-del-producto.md)
- [Tecnologías y arquitectura](docs/tecnologias-y-arquitectura.md)
- [Estado y hoja de ruta](docs/estado-y-hoja-de-ruta.md)
- [Presentación breve](docs/presentacion.md)

## Capturas

1. Pantalla de inicio (a) y gestión de capturas (b).


<img width="240" height="520" alt="fotoapp1" src="https://github.com/user-attachments/assets/6460324c-a3df-446f-8087-f2a64dfcd453" />

<img width="240" height="520" alt="fotoapp5" src="https://github.com/user-attachments/assets/6663e5bb-26ac-4c9f-8cab-91625835f8b0" />


2. Pantalla de amigos (ranking, solicitudes, amistades)


<img width="240" height="520" alt="fotoapp2" src="https://github.com/user-attachments/assets/765a2741-ca3a-459a-835a-c4720a2558d0" />
<img width="240" height="520" alt="fotoapp3" src="https://github.com/user-attachments/assets/56a2ba42-0f28-483b-9c9e-c1c73a376a66" />


3. Pantalla de estadísticas


<img width="240" height="520" alt="fotoapp4" src="https://github.com/user-attachments/assets/e57f053d-ae8b-4dfa-9287-a27dc171b991" />
<img width="240" height="520" alt="fotoapp5" src="https://github.com/user-attachments/assets/292f89ee-7b9e-4d0e-8dc1-60eb0e6acfdf" />


---

*PescaLog está en desarrollo. La descripción refleja la información disponible del proyecto y no implica que exista una versión de producción.*

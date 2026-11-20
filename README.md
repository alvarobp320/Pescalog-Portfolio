# PescaLog

> **Una app móvil para organizar y registrar la actividad de pesca.**

PescaLog es un proyecto personal en desarrollo que explora cómo llevar la experiencia de pesca al móvil: reunir la información de cada salida, facilitar el seguimiento de la actividad y construir una base preparada para crecer.

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

Las jornadas de pesca generan datos y recuerdos que pueden quedar dispersos. PescaLog busca ofrecer un lugar práctico desde el que registrar y consultar esa actividad, con una experiencia móvil sencilla y una arquitectura cliente-servidor que permita evolucionar el producto.

El alcance funcional continúa en construcción. Este portfolio evita presentar como terminadas funciones que todavía no han sido verificadas como parte de una versión publicada.

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

Las capturas de pantallas reales se añadirán cuando se prepare una selección de la app. Por ahora no se muestran imágenes de ejemplo para evitar confundir diseños conceptuales con pantallas implementadas.

## Enlaces

- [Repositorio de portfolio](https://github.com/alvarobp320/Pescalog-Portfolio)

---

*PescaLog está en desarrollo. La descripción refleja la información disponible del proyecto y no implica que exista una versión de producción.*
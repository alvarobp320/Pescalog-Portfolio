# PescaLog — visión del producto

## Resumen

PescaLog es una aplicación móvil en desarrollo cuyo objetivo es ayudar a las personas aficionadas a la pesca a organizar y consultar la información relacionada con sus capturas, así como ver estadísticas, gestionar amistades y competir por el top en el ranking.

La propuesta parte de una necesidad cotidiana: conservar en un mismo lugar los datos que hacen útil cada jornada y poder volver a ellos con facilidad. El producto se encuentra en fase de construcción, por lo que esta visión describe la dirección del proyecto y una lista de funciones testeadas pero que aún no están publicadas.

## Problema que aborda

La falta de seguimiento o pruebas de nuestras capturas de pesca, repartidas entre fotografías perdidas por la galería y recuerdos dispersos.

PescaLog plantea una experiencia móvil que permita centralizar esos registros y sentar las bases para consultar la actividad, datos y amistades.

## Para quién

Personas que practican la pesca y quieren mantener un registro personal de sus jornadas desde el teléfono, así como competir con gente de su entorno. 

El perfil, las necesidades y los casos de uso se podrán concretar mediante pruebas con usuarios.

## Principios de experiencia

- **Rápida en el contexto de uso:** pensada para consultarse desde un móvil.
- **Clara:** priorizar la información útil y una navegación comprensible.
- **Personal:** el registro pertenece a cada usuario. Solo comparte datos de tamaño y cantidad con sus amigos a elección.
- **Evolutiva:** separar la aplicación móvil de los servicios y datos permite ampliar el producto progresivamente.

## Alcance previsto

La versión actual dispone de funcionalidades de registro e inicio de sesión con autenticación JWT, gestión de usuarios y operaciones CRUD para las capturas. También incluye endpoints para consultar los catálogos de especies y señuelos.

El backend y sus APIs están implementados y probados mediante Postman, y la aplicación móvil ya se ejecuta correctamente en emuladores Android e iOS. La integración completa entre frontend y backend, así como la persistencia de sesión y el despliegue en un entorno de producción, forman parte de las siguientes etapas de desarrollo.

Funcionalidades como mapas, información meteorológica, comunidad, rankings y estadísticas avanzadas quedan fuera del alcance funcional actual y se contemplan como posibles ampliaciones futuras.

## Cómo valorar el proyecto

PescaLog permite mostrar el desarrollo de un producto digital de principio a fin, desde el diseño de su arquitectura hasta la implementación de una aplicación móvil conectada a un backend y una base de datos relacional.

El proyecto abarca tecnologías y conceptos como:
- Desarrollo backend con Java y Spring Boot.
- Diseño de APIs REST y gestión de operaciones CRUD.
- Persistencia de datos con PostgreSQL y Spring Data JPA.
- Autenticación y autorización mediante Spring Security y JWT.
- Desarrollo móvil multiplataforma con React Native y Expo.
- Separación de responsabilidades, organización por capas y gestión de DTOs.
- Control de versiones y documentación mediante Git y GitHub.
Además, representa una oportunidad para aplicar buenas prácticas de desarrollo, mejorar la experiencia de usuario y trabajar en aspectos como seguridad, pruebas, integración y despliegue.

## Próxima validación

1. Completar la integración frontend-backend: conectar las pantallas de registro, inicio de sesión y gestión de capturas con las APIs existentes.
2. Implementar la gestión de sesión: almacenar el JWT de forma segura, mantener la sesión del usuario y gestionar su expiración.
3. Validar los flujos funcionales: comprobar el registro, autenticación y operaciones sobre capturas desde la propia aplicación.
4. Reforzar seguridad y pruebas: verificar los permisos de usuario y administrador, el aislamiento de los datos y el comportamiento ante errores.
5. Preparar el despliegue: configurar un entorno remoto para el backend y PostgreSQL, gestionar las variables de entorno y preparar el almacenamiento de imágenes.
6. Preparar una primera versión de prueba: realizar pruebas en dispositivos reales Android e iOS, documentar resultados y recoger feedback.

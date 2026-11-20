# Tecnologías y arquitectura

## Arquitectura prevista

PescaLog se organiza en tres piezas:

1. **Aplicación móvil**: interfaz para Android e iOS, desarrollada con React Native y Expo.
2. **API**: backend en Java que recibe las peticiones del cliente y aplica la lógica de negocio.
3. **Base de datos**: PostgreSQL para persistir la información.

La aplicación móvil se comunica con la API. El backend es responsable de acceder a PostgreSQL; las credenciales de la base de datos no deben incluirse en la aplicación móvil.

```text
App móvil (React Native / Expo)
              │
              │ HTTPS · API
              ▼
        Backend Java
              │
              │ conexión privada
              ▼
         PostgreSQL
```

## Tecnologías del cliente

| Tecnología | Papel en el proyecto |
|---|---|
| React Native | Construcción de interfaces móviles para Android e iOS |
| Expo | Herramientas para desarrollar y preparar la aplicación |
| Expo Router | Navegación basada en rutas |
| Expo SecureStore | Almacenamiento local seguro disponible para datos de sesión |

La configuración revisada en el proyecto móvil indica Expo SDK 58 y React Native 0.88.1 como versiones objetivo declaradas. Las versiones pueden cambiar durante el desarrollo y deben confirmarse con el estado actual del repositorio de la app.

## Tecnologías del servidor y datos

| Tecnología | Papel en el proyecto |
|---|---|
| Java | Lenguaje del backend |
| API HTTP | Comunicación entre el móvil y el backend |
| JWT | Autenticación prevista para las solicitudes |
| PostgreSQL | Almacenamiento relacional |

Los chats disponibles describen el backend como Java. El framework concreto del servidor aún no queda confirmado en la documentación consultada, así que no se atribuye aquí Spring Boot ni otra tecnología específica.

## Seguridad y operación

- La app se conectará a la API mediante HTTPS cuando exista un entorno desplegado.
- Las credenciales de PostgreSQL se guardarán en la configuración privada del servidor.
- El backend validará la sesión mediante JWT según el flujo previsto.
- La app móvil no se conectará directamente a PostgreSQL.
- Conviene separar los entornos de pruebas y producción antes de publicar.

## Estado de despliegue

El diseño de despliegue sigue pendiente. En la información disponible, el backend y PostgreSQL se ejecutan localmente y no se confirma una API pública. Tampoco se confirma que exista una build distribuida en tiendas.

## Decisiones pendientes

- Framework y configuración definitiva del backend.
- Proveedor de alojamiento de la API y PostgreSQL.
- Dominio y certificado HTTPS.
- Gestión de secretos y copias de seguridad.
- Configuración de compilaciones de prueba y producción.
- Requisitos de privacidad, tratamiento de ubicación y publicación en tiendas.

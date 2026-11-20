# Estado y hoja de ruta

## Estado del proyecto

**Fase: desarrollo inicial; backend funcional en local y frontend en configuración e integración inicial.**

PescaLog se está desarrollando como una aplicación móvil multiplataforma con React Native y Expo, un backend Java con Spring Boot y PostgreSQL.

### Backend

- API REST desarrollada con Java y Spring Boot.
- PostgreSQL configurado y utilizado en entorno local.
- Registro de usuarios probado mediante Postman.
- Inicio de sesión probado mediante Postman; devuelve un JWT.
- Spring Security configurado para proteger los endpoints mediante JWT.
- Endpoints para consultar y gestionar capturas desarrollados y probados desde Postman.
- Roles `USER` y `ADMIN` incorporados al modelo y al JWT. La autorización completa de ADMIN sobre los recursos de otros usuarios sigue pendiente de terminar y probar.

### Frontend

- Proyecto React Native con Expo creado.
- La aplicación se ha ejecutado en Android mediante un emulador y en iPhone mediante Expo Go.
- La estructura inicial del cliente está preparada.
- La integración de las pantallas con la API, el almacenamiento seguro del JWT y la gestión de sesión están pendientes.

### Distribución e infraestructura

No hay todavía una versión de producción, una API pública, una base de datos alojada ni una publicación en App Store o Google Play. El backend y PostgreSQL se utilizan en local.

## Hoja de ruta propuesta

### 1. Consolidar el producto

- Definir los casos de uso y el alcance de la primera versión.
- Acordar qué información guarda cada captura.
- Diseñar y revisar los flujos principales de navegación.
- Priorizar para la primera versión: registro, inicio de sesión, perfil y gestión de capturas.
- Dejar funcionalidades secundarias —como amigos, rankings y meteorología— para iteraciones posteriores.
- Recoger comentarios de personas aficionadas a la pesca.

### 2. Completar la integración

- Mantener un contrato claro entre la app y la API: rutas, cuerpos de petición, respuestas y errores.
- Implementar las pantallas de Login y Register.
- Conectar React Native con Spring Boot mediante el cliente HTTP.
- Guardar el JWT de forma segura con Expo SecureStore y recuperar la sesión al volver a abrir la app.
- Mostrar la información del usuario y sus capturas.
- Completar desde el frontend la creación, consulta, edición y eliminación de capturas.
- Implementar estados de carga, estados vacíos, validaciones y mensajes de error comprensibles.
- Verificar que cada usuario solo puede acceder a sus propios datos y completar las reglas de acceso de ADMIN.

### 3. Preparar datos y despliegue

- Verificar y documentar el entorno local de PostgreSQL.
- Crear una base de datos alojada para pruebas.
- Configurar los secretos fuera del repositorio y del cliente móvil.
- Preparar el almacenamiento de imágenes de las capturas (por ejemplo, Cloudinary).
- Desplegar la API con HTTPS.
- Comprobar persistencia, copias de seguridad y recuperación de datos.
- Mantener separados los entornos de desarrollo, pruebas y producción.
- Configurar CORS y las variables de entorno necesarias para cada entorno.

### 4. Probar y preparar distribución

- Probar los flujos completos en dispositivos Android e iOS.
- Verificar autenticación, autorización y aislamiento de datos entre usuarios.
- Probar la subida y consulta de imágenes.
- Corregir problemas de usabilidad, compatibilidad y estabilidad.
- Preparar iconos, capturas reales, textos y política de privacidad.
- Generar builds de prueba y, cuando corresponda, enviarlas a revisión de las tiendas.

## Criterios para considerar lista una primera versión de prueba

- Los flujos acordados se completan de principio a fin desde la aplicación móvil.
- La app se comunica con un backend accesible y autenticado.
- El JWT se almacena de forma segura y la sesión se recupera correctamente.
- Un usuario no puede consultar, modificar ni eliminar capturas pertenecientes a otro usuario.
- Los permisos de ADMIN están implementados y probados según las reglas definidas.
- Los datos continúan disponibles después de reiniciar la app y los servicios.
- Las imágenes permanecen disponibles y vinculadas a su captura.
- Los errores de conexión y validación se presentan de forma comprensible.
- Las credenciales y secretos no se incluyen en el cliente ni en el repositorio.
- La aplicación se prueba en dispositivos Android e iOS.
- Hay capturas reales y una guía breve de uso.

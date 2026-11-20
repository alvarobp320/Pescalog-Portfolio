# Estado y hoja de ruta

## Estado del proyecto

**Fase: desarrollo inicial.**

La app móvil se ha ejecutado en Android mediante Expo. La arquitectura definida contempla una app React Native, un backend Java y PostgreSQL. La autenticación con JWT está planteada, pero no hay evidencia disponible de que el flujo completo esté terminado y desplegado.

No se confirma una versión de producción, una API pública, una base de datos alojada ni una publicación en App Store o Google Play.

## Hoja de ruta propuesta

### 1. Consolidar el producto

- Definir los casos de uso de la primera versión.
- Acordar qué información guarda cada registro.
- Diseñar y revisar los flujos principales de navegación.
- Recoger comentarios de personas aficionadas a la pesca.

### 2. Completar la integración

- Acordar el contrato entre la app y la API.
- Completar el inicio de sesión y la gestión de sesión.
- Conectar las pantallas con el backend.
- Definir validaciones, estados vacíos y mensajes de error.

### 3. Preparar datos y despliegue

- Restaurar y verificar el entorno local de PostgreSQL.
- Crear una base de datos alojada para pruebas.
- Configurar secretos en el servidor.
- Desplegar la API con HTTPS y comprobar persistencia y recuperación.
- Mantener entornos de pruebas y producción separados.

### 4. Probar y preparar distribución

- Probar los flujos con usuarios y dispositivos reales.
- Corregir problemas de usabilidad y estabilidad.
- Preparar iconos, capturas, textos y política de privacidad.
- Generar builds de prueba y, cuando corresponda, enviarlas a revisión de las tiendas.

## Criterios para considerar lista una primera versión de prueba

- Los flujos acordados se completan de principio a fin.
- La app se comunica con un backend accesible y autenticado.
- Los datos continúan disponibles después de reiniciar la app y el servicio.
- Los errores de conexión y validación se presentan de forma comprensible.
- Las credenciales y secretos no se incluyen en el cliente ni en el repositorio.
- Hay capturas reales y una guía breve de uso.

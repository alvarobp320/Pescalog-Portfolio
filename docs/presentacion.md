# PescaLog — presentación breve

## 1. El proyecto

**PescaLog** es una app móvil en desarrollo para gestionar tus capturas de pesca, comprobar tus estadísticas, así como tener y gestionar amistades con otros usuarios y competir por el ranking.

## 2. La necesidad

¿De dónde sale la idea de Pescalog? 

El objetivo era cumplir un "problema" que solía aparecer cuando hablaba con compañeros sobre nuestras capturas de pesca. Se hacía complicado recordar la información como el peso, el señuelo utilizado, tamaño... Y al final, estábamos minutos y minutos tratando de encontrar una fotografía que corroborase que no exagerábamos o mentíamos.

Entonces, cuando en mi cumpleaños me regalaron una agenda de pesca (en la que tenías huecos para poner el tamaño, especie, hora del día, etc.), la usé continuamente en mis jornadas de pesca. Pero tras poco tiempo, se hacía incómodo y la agenda acababa mojada y sucia, por lo que pensé: ¿Por qué no hacer una agenda digital con más datos, fotografías y amistades? Y así, de forma resumida, surgió Pescalog.

## 3. La experiencia

El producto se está planteando para móvil, con una navegación sencilla y directa, siendo una experiencia que pueda evolucionar a partir de las necesidades de quienes pescan.

## 4. Cómo está construida

- **Móvil:** React Native y Expo.
- **Servidor:** Java y una API HTTP.
- **Datos:** PostgreSQL.
- **Sesión:** autenticación basada en JWT prevista en la arquitectura, así como funciones de Spring Security.

La app se comunica con el backend, y el backend gestiona el acceso a la base de datos.

## 5. Estado actual

La aplicación se ha iniciado en emuladores Android con Expo y en mi móvil Iphone en Expo Go. La solución todavía está en desarrollo: no tiene despliegue público confirmado ni está publicada en las tiendas.

En la prueba podemos utilizar todas las APIs -> Crear cuentas, logearnos, gestionar nuestras capturas (CRUD), amistades y ver rankings.

## 6. Próximos pasos

Concretar el alcance de la primera versión, completar la integración móvil-API, preparar un entorno de pruebas alojado, validar los flujos y reunir capturas reales del producto.

Corregir y mejorar la UX/UI, así como implementar nuevas funcionalidades como el modo oscuro, implementación de subida de fotografías e incluso una IA que detecte especies en base a fotos del usuario.

## Mensaje de cierre

PescaLog es un proyecto en evolución que combina lo aprendido en el Ciclo Superior de Desarrollo de Aplicaciones Multiplataforma, lo aprendido de forma autodidacta y lo aprendido en las prácticas de ViewNext.

El resultado, aunque aún no finalizado, es una aplicación con un backend en Java seguro, estable y escalable gracias al uso de la arquitectura hexagonal, el framework de Spring Boot, Spring Security, JWT, comprobaciones y validaciones en back-bbdd-front, entre otros.

---

**Portfolio:** [github.com/alvarobp320/Pescalog-Portfolio](https://github.com/alvarobp320/Pescalog-Portfolio)

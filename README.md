# Puntos de Acopio - Sismo Colombia

SPA estática para Netlify que muestra puntos de acopio y permite registrar reportes comunitarios en tiempo real con Firebase Firestore.

## Activar datos en tiempo real

1. Crea un proyecto en [Firebase](https://console.firebase.google.com/).
2. Crea una base de datos **Cloud Firestore** en modo producción.
3. Publica las reglas de `firestore.rules` en Firestore Rules.
4. En `index.html`, reemplaza los valores `REEMPLAZA_CON_*` dentro de `firebaseConfig` por la configuración web de tu proyecto.
5. Sube el repositorio a Netlify. No requiere build command; el archivo principal es `index.html`.

Mientras `firebaseConfig` tenga placeholders, la app funciona en modo demo: muestra los puntos iniciales y permite agregar registros temporales solo en la sesión actual del navegador.

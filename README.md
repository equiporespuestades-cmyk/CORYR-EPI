# CORYR EPI 8.3 — Android

Aplicación Android WebView para https://epinvestiga.equipo-respuesta-des.workers.dev/

## Compilación desde GitHub (sin PC)
1. Crea un repositorio privado nuevo en GitHub.
2. Sube **todo el contenido de esta carpeta** (incluida `.github/workflows/android-apk.yml`) a la raíz del repositorio.
3. Abre Actions → Compilar APK Android → Run workflow (o realiza un push a main).
4. Cuando termine correctamente, abre la ejecución → Artifacts → descarga `CORYR-EPI-8.3-Android-APK`.
5. Descomprime el ZIP de GitHub, instala `app-debug.apk` en Android. Autoriza la instalación desde esa fuente cuando el sistema lo solicite.

## Alternativa Android Studio
Abre la carpeta como proyecto Android y selecciona Build → Build APK(s).

## Notas
- Es una versión de prueba (debug), no un APK firmado para Play Store.
- Requiere internet. Supabase funcionará solamente si la web publicada ya está configurada correctamente.
- La geolocalización requiere autorización del usuario y, tras la primera autorización, puede requerir recargar la página.
- No incluye credenciales ni claves Supabase en el código Android.
- Para distribución institucional, agregar autenticación, reglas RLS, políticas de privacidad y firma release.

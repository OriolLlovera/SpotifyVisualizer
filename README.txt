SPOTIFY VISUALIZER — Instrucciones de despliegue en Netlify
============================================================

1. SUBE ESTA CARPETA A NETLIFY
   - Ve a netlify.com → "Add new site" → "Deploy manually"
   - Arrastra toda esta carpeta (spotify-viz-netlify) al área de deploy
   - Netlify te dará una URL tipo: https://tu-app.netlify.app

2. AÑADE TU CLIENT ID COMO VARIABLE DE ENTORNO
   - En Netlify: Site settings → Environment variables → Add variable
   - Nombre:  SPOTIFY_CLIENT_ID
   - Valor:   97a16e5acf0c45c38b2e0c12184fcd4b

3. ACTUALIZA LA REDIRECT URI EN SPOTIFY DEVELOPER
   - Ve a developer.spotify.com/dashboard → tu app → Settings
   - Añade como Redirect URI: https://TU-DOMINIO.netlify.app/
     (con la barra final, es la raíz del sitio)
   - Guarda

4. REDEPLOY
   - En Netlify haz un nuevo deploy para que coja la variable de entorno

¡Listo! Cualquier persona que abra la web verá el botón "Conectar con Spotify".

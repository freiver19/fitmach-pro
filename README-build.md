FitMachPro - proyecto con mapas (dev) y notificaciones push (FCM)

Pasos principales:
1) npm install
2) Para Maps en desarrollo (ionic serve): añade en src/index.html dentro de <head> la linea:
   <script src="https://maps.googleapis.com/maps/api/js?key=TU_API_KEY&libraries=places"></script>
3) Para Push: npm install @capacitor/push-notifications firebase @angular/fire
   npx cap add android
   npx cap add ios
   Copia google-services.json a android/app/ y GoogleService-Info.plist a ios/App/
   npx cap sync
4) Ejecuta ionic serve (web demo) o ionic capacitor run android --livereload

Modo demo: usa localStorage (demo_offers, demo_users) para probar sin Firebase.!
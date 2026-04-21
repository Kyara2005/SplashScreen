# 📸 Photo Gallery con Splash Screen e Icono personalizado
<img width="512" height="512" alt="icon-only" src="https://github.com/user-attachments/assets/e40eb50a-da47-40e3-a605-44a0f66ba23c" />

## 📌 Descripción

Aplicación móvil desarrollada con Ionic + Capacitor que implementa:

* Splash Screen personalizado
* Icono adaptativo
* Navegación por tabs

---

## ⚙️ Tecnologías utilizadas

* Ionic
* Capacitor
* Android Studio

---
## 🖼️ Implementación del Splash Screen

### 📚 Documentación oficial

Para obtener un Splash Screen exitoso se puede encontrar la documentación adecuada en los siguientes links:

* [Splash Screen API](https://capacitorjs.com/docs/apis/splash-screen)
* [Splash & Icons Guide](https://capacitorjs.com/docs/guides/splash-screens-and-icons)

---

### 🔧 Configuración en `capacitor.config.ts`

Después de la instalación, hay que implementar lo siguiente

```ts
"plugins": {
  "SplashScreen": {
    "launchShowDuration": 3000,
    "launchAutoHide": true,
    "launchFadeOutDuration": 3000,
    "backgroundColor": "#ffffffff",
    "androidSplashResourceName": "splash",
    "androidScaleType": "CENTER_CROP",
    "showSpinner": true,
    "androidSpinnerStyle": "large",
    "iosSpinnerStyle": "small",
    "spinnerColor": "#999999",
    "splashFullScreen": true,
    "splashImmersive": true,
    "layoutName": "launch_screen",
    "useDialog": true
  }
}
```

<img width="680" height="803" alt="image" src="https://github.com/user-attachments/assets/8e31f1d3-f6fb-4a25-ae0f-d9a659a49956" />

---

### 📁 Recursos necesarios

Crear una carpeta `assets/` con:

* icon-only.png
* icon-foreground.png
* icon-background.png
* splash.png
* splash-dark.png

📌 Nota: Puedes usar herramientas como **Ape Tools** para ajustar tamaños.

---

### 🎨 Configuración en Android

Hay que ubicarse en: `res/values/styles.xml`

```xml
<style name="AppTheme.NoActionBarLaunch" parent="AppTheme.NoActionBar">
    <item name="android:background">@drawable/splash</item>
</style>
```

📷 Ejemplo:

<img width="998" height="264" alt="image" src="https://github.com/user-attachments/assets/1c333e48-9b37-47bf-9852-29e10fe85279" />

Y listo, con el comando ionic cap add android, ya se puede configurar para ese sistema

---

## 📱Visualización final

### 📦Instalación del apk

<img width="698" height="1600" alt="image" src="https://github.com/user-attachments/assets/e4d74ed4-4b79-4864-b654-da479d6ca3ee" />

### 📲Icono en pantalla

<img width="246" height="343" alt="image" src="https://github.com/user-attachments/assets/922ecca3-01ec-439c-a82b-4f95c63bcc0a" />

### 🔓 Apertura de la app

<img width="1080" height="2412" alt="image" src="https://github.com/user-attachments/assets/75d5932d-360b-4bb7-bda5-55617ca9ac22" />

### 📑 Navegación por tabs:

<img width="1080" height="2412" alt="image" src="https://github.com/user-attachments/assets/7ce7b1bd-28e4-4c34-9d20-484dd5ef6897" />
<img width="1080" height="2412" alt="image" src="https://github.com/user-attachments/assets/87333ef1-70ab-41d5-a586-4345aa83cd5a" />
<img width="716" height="1600" alt="image" src="https://github.com/user-attachments/assets/6e92352e-272c-4856-9460-2ceaadb41a30" />

## ✅ Conclusión

Se obtuvo una excelente visualización del sistema con el Splash screen y el icono personalizado que caracteriza a la app y mejora la experiencia visual del usuario.

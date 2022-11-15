Para ejecutar:

1. npm install

2. Puedes configurar tu propia licencia en el archivo `src\app\scanner\scanner.page.html`.

   ```html
   <app-barcode-scanner
     [isActive] = "isActive"
     [runtimeSettings] = "runtimeSettings"
     [torchOn] = "torchOn"
     dbrLicense = "DLS2eyJoYW5kc2hha2VDb2RlIjoiMjAwMDAxLTE2NDk4Mjk3OTI2MzUiLCJvcmdhbml6YXRpb25JRCI6IjIwMDAwMSIsInNlc3Npb25QYXNzd29yZCI6IndTcGR6Vm05WDJrcEQ5YUoifQ=="
     dceLicense = "DLS2eyJoYW5kc2hha2VDb2RlIjoiMjAwMDAxLTE2NDk4Mjk3OTI2MzUiLCJvcmdhbml6YXRpb25JRCI6IjIwMDAwMSIsInNlc3Npb25QYXNzd29yZCI6IndTcGR6Vm05WDJrcEQ5YUoifQ=="
     (onFrameRead)="onFrameRead($event)">
   </app-barcode-scanner>
   ```
   
   [Obtén una licencia de prueba de Dynamsoft aquí](https://www.dynamsoft.com/customer/license/trialLicense/?product=dbr).

3. Añadir plataformas a Cordova: 

   ```
   ionic cordova platforms add android
   ionic cordova platforms add ios
   ```
   
4. Prepara el proyecto para las plataformas elegidas:

   ```
   ionic cordova prepare android
   ionic cordova prepare ios
   ```
   
5. ¡Listo! Para poder probar el escáner, instala la app en un dispositivo Android utilizando el instalador .apk generado por Android Studio.


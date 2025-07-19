## **Explorando Arduino: Tu Primer Programa en Arduino UNO**

#### **Conexión Inicial**
1. Conecta tu placa Arduino UNO al puerto USB de tu ordenador, estableciendo el primer vínculo entre la creatividad y la tecnología.
2. Abre con entusiasmo el programa Arduino IDE, tu herramienta para esculpir el futuro digital.

#### **Configuración del Entorno**
3. En el menú superior, navega hasta la opción "Herramientas" y elige la placa "Arduino UNO".
4. Selecciona el puerto COM de la placa en la misma sección de herramientas, garantizando una comunicación fluida.


#### **LED 13: El Protagonista**
6. Observa el LED amarillo que ilumina cuando conectas la placa. Al lado, el LED rojo marcado con la letra L, asociado al pin digital 13, será nuestro lienzo para la creación.
7. Para encender y apagar este LED, emplearemos las siguientes instrucciones:

   - Encender LED: `digitalWrite(13, HIGH);`
   - Apagar LED: `digitalWrite(13, LOW);`

#### **Programa Inicial: Luces Intermitentes**
8. Es momento de dar vida al LED 13 con un programa inicial. Vamos a crear un bucle de instrucciones que hará parpadear el LED. Aquí está el código mágico:

```arduino
void setup() {
  pinMode(13, OUTPUT);
}

void loop() {
  digitalWrite(13, HIGH);
  delay(500);
  digitalWrite(13, LOW);
  delay(500);
}
```

#### **Guardando y Desatando la Magia**
9. Una vez escrito este código, guárdalo en tu PC y prepárate para el momento emocionante.
10. Sube el programa a la placa pulsando el segundo ícono en el menú. ¡Desata la magia digital!

#### **Verificando el Éxito**
11. Si el programa se almacena correctamente, te recibirán las palabras "subido". En la placa, un LED parpadeará, anunciando tu éxito en el mundo Arduino.

### **¡Felicidades, Has Hecho Magia!**
Has creado y cargado tu primer programa en Arduino UNO. Este es solo el comienzo de una travesía emocionante. ¡Explora, experimenta y que la magia Arduino te guíe hacia nuevos horizontes electrónicos! 🌟💻🚀

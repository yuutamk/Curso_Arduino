# Control de LEDs con Arduino

Utilizaremos un ciclo **for** para alternar entre los LEDs amarillo y rojo.

### Materiales
- Arduino (cualquier modelo)
- 2 LEDs (uno amarillo y otro rojo)
- Resistencias (220 ohmios)
- Protoboard y cables de conexión

### Esquema de Montaje
Conecta los componentes siguiendo el siguiente esquema:

1. Conecta el LED amarillo al **pin 13** del Arduino.
2. Conecta el LED rojo al **pin 12** del Arduino.
3. Añade una resistencia de **220 ohmios** en serie con cada LED (conectada al pin positivo del LED).
4. Conecta el pin negativo de ambos LEDs al **GND** del Arduino.

![](../src/Practics/leds%20amarillo%20y%20rojo.png)

### Código
```cpp
int yellowPin = 13;
int redPin = 12;
int dt = 500;
int yellow = 3;
int red = 5;
int i;

void setup() {
  pinMode(yellowPin, OUTPUT);
  pinMode(redPin, OUTPUT);
}

void loop() {
  for (i = 1; i <= yellow; i++) {
    digitalWrite(yellowPin, HIGH);
    delay(dt);
    digitalWrite(yellowPin, LOW);
    delay(dt);
  }

  for (i = 0; i < red; i++) {
    digitalWrite(redPin, HIGH);
    delay(dt);
    digitalWrite(redPin, LOW);
    delay(dt);
  }
}
```

### Explicación
1. **Configuración**: En la función **setup()**, establecemos los pines **yellowPin** y **redPin** como salidas.
2. **Bucle principal**: En la función **loop()**, utilizamos dos bucles **for**:
   - El primer bucle enciende y apaga el LED amarillo **3 veces**.
   - El segundo bucle enciende y apaga el LED rojo **5 veces**.

### Resultado
Al cargar este código en tu Arduino, verás cómo los LEDs amarillo y rojo se encienden y apagan alternadamente.

# Medición de Voltaje con Arduino


En esta práctica, aprenderemos cómo medir el voltaje utilizando un Arduino y una resistencia. El objetivo es leer el voltaje en el pin analógico A0 y convertirlo en una lectura comprensible.

### Esquematico
![](../src/Practics/voltimetro%20analogico.png)

### Materiales
- Arduino (cualquier modelo compatible)
- Resistencia (cualquier valor)
- Protoboard
- Cables de conexión
- Computadora con el IDE de Arduino instalado

### Paso 1: Configuración
Primero, definimos las variables necesarias:

```cpp
int analogPin = A0; // Pin analógico A0
float V2; // Voltaje calculado
int dt = 500; // Retardo en milisegundos
int analogVal; // Valor leído del pin analógico
```

- `analogPin`: El pin analógico A0 se utilizará para leer el voltaje.
- `V2`: Almacenará el voltaje calculado.
- `dt`: El tiempo de retardo entre lecturas.
- `analogVal`: Almacenará el valor leído del pin analógico.

### Paso 2: Configuración Inicial
En la función `setup()`, configuramos el pin A0 como entrada y habilitamos la comunicación serial:

```cpp
void setup() {
  pinMode(analogPin, INPUT); // Configurar A0 como entrada
  Serial.begin(9600); // Iniciar comunicación serial a 9600 bps
}
```

### Paso 3: Lectura y Cálculo del Voltaje
En la función `loop()`, leemos el valor analógico, lo convertimos a voltaje y lo imprimimos en el monitor serial:

```cpp
void loop() {
  analogVal = analogRead(analogPin); // Leer valor analógico
  V2 = (5.0 * analogVal) / 1023.0; // Calcular voltaje (escala de 0 a 5V)
  Serial.println(V2); // Imprimir voltaje
  delay(dt); // Esperar antes de la siguiente lectura
}
```

- `analogRead(analogPin)`: Lee el valor analógico del pin A0.
- `V2 = (5.0 * analogVal) / 1023.0`: Calcula el voltaje utilizando la relación entre el valor leído y la escala de 0 a 5V.
- `Serial.println(V2)`: Imprime el voltaje en el monitor serial.
- `delay(dt)`: Espera antes de la siguiente lectura.

### Resultado
Al cargar este código en tu Arduino y conectar una resistencia al pin A0, podrás ver el voltaje medido en el monitor serial. ¡Experimenta con diferentes resistencias y observa cómo cambia el voltaje!
 🤖🔌
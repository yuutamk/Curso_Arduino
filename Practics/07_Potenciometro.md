# Control de Intensidad de LED con Arduino y un Potenciómetro


## Materiales Necesarios
- Placa Arduino (Arduino Uno)
- LED (cualquier color)
- Resistencia de 220 ohmios
- Potenciómetro (también conocido como potenciómetro variable o perilla giratoria)
- Cables de conexión

## Esquematico
![](../src/Practics/potenciometro%20%202.png)

## El Código

Aquí está el código que utilizaremos para esta práctica:

```cpp
int LED = 3;
int BRILLO;
int POT = 0;

void setup() {
  pinMode(LED, OUTPUT);
  // Las entradas analógicas no requieren inicialización
}

void loop() {
  BRILLO = analogRead(POT) / 4;
  analogWrite(LED, BRILLO);
}
```

## Explicación

1. **Declaración de variables:**
   - `LED`: Representa el pin al que está conectado el LED.
   - `BRILLO`: Almacena el valor de brillo calculado a partir de la lectura del potenciómetro.
   - `POT`: Representa el pin analógico al que está conectado el potenciómetro.

2. **Configuración inicial:**
   - En la función `setup()`, configuramos el pin del LED como una salida digital.
   - No es necesario inicializar los pines analógicos, ya que Arduino los configura automáticamente.

3. **Bucle principal:**
   - En la función `loop()`, leemos el valor analógico del potenciómetro utilizando `analogRead(POT)`.
   - Dividimos este valor por 4 para ajustar el rango de brillo (puedes ajustar este factor según tus necesidades).
   - Finalmente, utilizamos `analogWrite(LED, BRILLO)` para establecer el brillo del LED.

## Montaje

1. Conecta el LED al pin 3 del Arduino.
2. Conecta el potenciómetro al pin analógico 0.
3. Asegúrate de conectar las resistencias necesarias para el LED (si es un LED estándar).

## Resultado

Al girar el potenciómetro, verás cómo el brillo del LED cambia gradualmente. ¡Experimenta con diferentes valores y observa cómo afecta la intensidad luminosa!


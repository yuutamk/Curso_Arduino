#  Cálculo del Área de un Círculo


En esta práctica, aprenderemos cómo calcular el área de un círculo utilizando la fórmula matemática adecuada. Utilizaremos un Arduino para realizar los cálculos y mostrar los resultados en el monitor serial.

### Materiales
- Arduino (cualquier modelo compatible)
- Computadora con el IDE de Arduino instalado

### Paso 1: Configuración Inicial

Primero, definimos las variables necesarias:
```arduino
int wait = 500; // Tiempo de retraso en milisegundos
float area; // Almacena el área calculada del círculo. 
float Pi = 3.1415;
int rad = 3; // Representa el radio del círculo.
String mensaje1 = "El area de un circulo con radio de ";
String mensaje2 = " es de: ";
// Son cadenas de texto que describen el proceso y el resultado. En este caso, se utilizan para imprimir mensajes en el monitor serial.
```

En la función `setup()`, simplemente iniciamos la comunicación serial:

```cpp
void setup() {
  Serial.begin(9600); // Iniciar comunicación serial a 9600 bps
}
```

### Paso 2: Cálculo del Área
En la función `loop()`, calculamos el área de un círculo con un radio fijo (en este caso, **3 unidades**):

```cpp
void loop() {
  float area = Pi * rad * rad; // Calcular el área del círculo
  Serial.print(mensaje1); // Imprimir el primer mensaje
  Serial.print(rad); // Imprimir el valor del radio
  Serial.print(mensaje2); // Imprimir el segundo mensaje
  Serial.println(area); // Imprimir el área calculada
  delay(wait); // Esperar antes de la siguiente iteración
  rad++; // Incrementar el radio para futuras iteraciones
}
```

- `Pi`: Es una aproximación del valor de π (pi) utilizado en la fórmula del área del círculo.
- `rad`: Representa el radio del círculo (inicialmente **3**).
- `area`: Almacena el área calculada.
- `mensaje1` y `mensaje2`: Son cadenas de texto que describen el proceso y el resultado.

### Resultado
Al cargar este código en tu Arduino, verás cómo se imprime el área del círculo en el monitor serial. Puedes modificar el valor del radio o experimentar con diferentes tamaños de círculos. ¡Diviértete explorando las matemáticas con Arduino! 🤖📏
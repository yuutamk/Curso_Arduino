# **Arduino: Más Allá de la Electrónica Convencional**

¡Bienvenidos, entusiastas de la electrónica y creadores de futuros brillantes! En este viaje por el fascinante mundo de Arduino, desentrañaremos sus raíces, exploraremos sus múltiples facetas y nos sumergiremos en la creación de nuestro propio proyecto. Prepara tu mente creativa, ¡comencemos!

![logo](/src/arduino-logo-0.png)

#### **¿Qué es Arduino?**
Arduino no es solo un microcontrolador; es una revolución creativa. Es una plataforma de hardware libre basada en un microcontrolador, principalmente Atmel AVR. Lo esencial: una PCB con todos los elementos necesarios. Pero la magia radica en su IDE libre y su lenguaje de programación propio, simplificado para acercar la electrónica a todos, sin importar los conocimientos previos o los recursos económicos.

![alt text](/src/image.png)

#### **Historia de Arduino: De Italia al Mundo**
El año 2005 marcó el nacimiento de Arduino en Italia. Estudiantes del Instituto de diseño Interactivo IVREA, buscando alternativas asequibles, crearon una plataforma basada en Atmel AVR. El proyecto, liderado por Massimo Banzi, David Cuartilles y Gianluca Martino, desplazó soluciones costosas del mercado, llevando la creatividad a nuevas alturas.

![alt text](/src/image-3.png)

#### **Innovación con Simplicidad: El Éxito de Arduino**
La sencillez de Arduino proviene de su IDE y el bootloader en el microcontrolador, permitiendo la programación directa mediante un simple cable USB. Compatible con diversos sistemas operativos, desde Windows hasta Linux y MacOS, Arduino se convierte en una herramienta accesible y poderosa para todos.

![alt text](/src/image-2.png)

#### **Arduino en Evolución: Más Allá del Comienzo**
Tras su lanzamiento, Arduino no dejó de evolucionar. Desde el Kit ADK de Google para comunicarse con smartphones Android hasta el desarrollo de placas Arduino 32 bit y contribuciones de Intel con la placa Galileo, el proyecto se expandió y diversificó. Incluso surgieron compatibles y sistemas similares, pero la esencia de Arduino persiste.

![ADK](/src/mega-adk.jpg)


#### **Modelos de Arduino: Un Universo de Posibilidades**
- **Arduino Uno:** La clásica. 
![uno](/src/ArduinoUno_R3_y_usb.webp)
- **Arduino Leonardo:** Con procesador ATmega32U4. 
![leonardo](/src/arduino-leonardo.2.jpg)
- **Arduino Due:** Potencia con ARM Cortex. 
![DUE](/src/arduino-due.png)
- **Arduino Yún:** Integración de Linux. 
![Yun](/src/ARDUINO_YUN.png)
- **Arduino Mega 2560:** Para proyectos extensos. 
![Mega](/src/arduino-mega.png)
- **Arduino Micro:** Pequeño pero poderoso. ![micro](/src/arduino-micro.jpg)
- **Arduino Nano:** Compacto y versátil. 
![nano](/src/arduino-nano.jpg)
- **Arduino Pro Mini, Fio, Esplora:** Adaptabilidad en diversas situaciones. 
![espora](/src/arduino-esplora.jpg)

#### **¿Qué Hacer con Arduino? ¡Todo es Posible!**
- **Automatización del hogar:** Luces, persianas, electrodomésticos.
![luces](/src/lucesled-arduino.webp)
- **Robótica:** Desde juguetes hasta proyectos complejos.
![robot](/src/elegoo-robot-car.jpg)
- **Arte interactivo:** Donde la creatividad se encuentra con la tecnología.
![guitar](/src/arduino-guitar.jpg)
- **Monitoreo con sensores:** Medición de temperatura, humedad, y más.
![sensores](/src/sensores.JPG)





#### **El Encanto del IDE Arduino**
El entorno de desarrollo de Arduino es una joya para los amantes de la programación. Basado en C y C++, su simplicidad lo hace accesible para principiantes, mientras que su potencia satisface a los expertos. ¡Programar con Arduino es una experiencia que engancha!
![IDE](/src/idearduino.webp)

#### **Arduino en la Educación y la Industria**
Desde aulas hasta fábricas, Arduino ha dejado huella. Su enfoque en la educación ha permitido que estudiantes de todas las edades se sumerjan en la electrónica y la programación de manera divertida y educativa. Además, en la industria, su versatilidad lo ha convertido en un aliado invaluable para la creación de prototipos y soluciones personalizadas.

![escuela](/src/arduino-escuela.jpg)

#### **Explorando Funciones y Librerías**
Las funciones de Arduino, desde la gestión de E/S digitales hasta el manejo del tiempo, abren un abanico de posibilidades para los creadores. Además, las librerías simplifican el control de distintos dispositivos, facilitando la integración de sensores, módulos y shields en nuestros proyectos.

### **¡Inspírate y Crea con Arduino!**
Arduino es la puerta de entrada a un universo de posibilidades. ¡Inspírate en la creatividad de Arduino, explora nuevos proyectos y deja que la innovación electrónica guíe tus creaciones! 🌌💡🛠️

## El Lenguaje de Programación de Arduino: C++ con un Toque Especial

Cuando hablamos del lenguaje de programación de Arduino, estamos principalmente en el territorio de **C++**. Pero espera, no te asustes si no eres un gurú de la programación. Aquí está la magia: **Arduino ha adaptado C++ para que sea más accesible y amigable para principiantes**. Así que, incluso si eres nuevo en esto, ¡no te preocupes!

### ¿Por qué C++?

- **Control Total**: C++ es un lenguaje estructurado y de alto nivel que te permite tener un mayor control sobre el hardware. Si eres un entusiasta de los detalles técnicos, C++ es tu amigo.
- **Eficiencia**: C++ está diseñado para ser eficiente en el uso de recursos. Esto significa que tus programas en Arduino serán rápidos y eficaces.

### ¿Qué es Wiring?

**Wiring** es el nombre del lenguaje de programación específico de Arduino. Está basado en C++ y viene con una serie de librerías y funciones que hacen que la programación sea más sencilla. Piensa en Wiring como el "idioma común" que conecta a los programadores con las placas Arduino.

## Las Piezas del Rompecabezas: Funciones, Variables y Constantes

### Funciones

Las funciones son como pequeños bloques de construcción que le dicen a Arduino qué hacer. Algunas funciones comunes incluyen:

- `digitalRead()`: Lee el estado de un pin digital.
- `analogWrite()`: Controla la intensidad de una señal analógica.

### Variables y Constantes

- **Variables**: Almacenan valores temporales (como temperaturas o estados).
- **Constantes**: Son valores fijos que no cambian durante la ejecución del programa.

## ¡Hora de Programar!

Aquí tienes un ejemplo sencillo de cómo encender un LED utilizando Arduino:

```cpp
void setup() {
  pinMode(LED_BUILTIN, OUTPUT); // Configura el pin del LED como salida
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH); // Enciende el LED
  delay(1000); // Espera 1 segundo
  digitalWrite(LED_BUILTIN, LOW); // Apaga el LED
  delay(1000); // Espera otro segundo
}
```

Este código configura el LED incorporado en la placa Arduino para que parpadee cada segundo. ¡Simple pero efectivo!

## El Lenguaje de Programación de Arduino: C++ con un Toque Especial

Cuando hablamos del lenguaje de programación de Arduino, estamos principalmente en el territorio de **C++**. Pero espera, no te asustes si no eres un gurú de la programación. Aquí está la magia: **Arduino ha adaptado C++ para que sea más accesible y amigable para principiantes**. Así que, incluso si eres nuevo en esto, ¡no te preocupes!

### ¿Por qué C++?

- **Control Total**: C++ es un lenguaje estructurado y de alto nivel que te permite tener un mayor control sobre el hardware. Si eres un entusiasta de los detalles técnicos, C++ es tu amigo.
- **Eficiencia**: C++ está diseñado para ser eficiente en el uso de recursos. Esto significa que tus programas en Arduino serán rápidos y eficaces.

### ¿Qué es Wiring?

**Wiring** es el nombre del lenguaje de programación específico de Arduino. Está basado en C++ y viene con una serie de librerías y funciones que hacen que la programación sea más sencilla. Piensa en Wiring como el "idioma común" que conecta a los programadores con las placas Arduino.

## Las Piezas del Rompecabezas: Funciones, Variables y Constantes

### Funciones

Las funciones son como pequeños bloques de construcción que le dicen a Arduino qué hacer. Algunas funciones comunes incluyen:

- `digitalRead()`: Lee el estado de un pin digital.
- `analogWrite()`: Controla la intensidad de una señal analógica.

### Variables y Constantes

- **Variables**: Almacenan valores temporales (como temperaturas o estados).
- **Constantes**: Son valores fijos que no cambian durante la ejecución del programa.

## ¡Hora de Programar!

Aquí tienes un ejemplo sencillo de cómo encender un LED utilizando Arduino:

```cpp
void setup() {
  pinMode(LED_BUILTIN, OUTPUT); // Configura el pin del LED como salida
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH); // Enciende el LED
  delay(1000); // Espera 1 segundo
  digitalWrite(LED_BUILTIN, LOW); // Apaga el LED
  delay(1000); // Espera otro segundo
}
```

Este código configura el LED incorporado en la placa Arduino para que parpadee cada segundo. ¡Simple pero efectivo!

## **Señales Analógicas en Arduino**

### **1. ¿Qué es una señal analógica?**
Antes de sumergirnos en las funciones, es importante entender qué es una señal analógica. A diferencia de las señales digitales que solo pueden tener dos estados (alto o bajo), las señales analógicas pueden tener **infinitos valores**. Por ejemplo, el voltaje en un enchufe de casa es una señal analógica que puede variar continuamente entre 0 y 220 voltios (o 120 voltios, según la región).

### **2. analogRead()**
La función `analogRead(pin)` se utiliza para **leer el valor analógico** de un pin específico. Esta función convierte la tensión en ese pin en un número entre 0 y 1023. Aquí tienes un ejemplo:

```arduino
int potPin = A0; // Pin analógico conectado al potenciómetro
int ledPin = 9; // LED conectado al pin digital 9
int val = 0; // Variable para almacenar el valor leído

void setup() {
  pinMode(ledPin, OUTPUT); // Configura el pin del LED como salida
}

void loop() {
  val = analogRead(potPin); // Lee el valor del potenciómetro
  analogWrite(ledPin, val / 4); // Controla el brillo del LED
}
```

En este ejemplo, el LED se iluminará proporcionalmente al valor leído del potenciómetro. Los valores de `analogRead` van de 0 a 1023, mientras que los valores de `analogWrite` van de 0 a 255.

### **3. analogWrite()**
La función `analogWrite(pin, value)` se utiliza para **escribir una señal PWM (modulación por ancho de pulso)** en un pin. Puede usarse para encender un LED a diferentes niveles de brillo o para controlar la velocidad de un motor. Por ejemplo:

```arduino
int ledPin = 6; // LED conectado al pin digital 6

void setup() {
  pinMode(ledPin, OUTPUT); // Configura el pin del LED como salida
}

void loop() {
  analogWrite(ledPin, 128); // Enciende el LED al 50% de brillo
  delay(1000); // Espera 1 segundo
  analogWrite(ledPin, 0); // Apaga el LED
  delay(1000); // Espera 1 segundo
}
```

En este caso, el LED se atenuará al 50% de brillo y luego se apagará alternativamente cada segundo.
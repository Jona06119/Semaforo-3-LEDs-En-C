# Semáforo con 3 LEDs en C (PIC16F877A)

Proyecto de sistemas embebidos que simula el funcionamiento de un semáforo utilizando un microcontrolador PIC16F877A[cite: 5] y programado en lenguaje C.

## Tecnologías y Herramientas
* **Microcontrolador**: PIC16F877A
* **Lenguaje**: C (para microcontroladores PIC)
* **Oscilador**: Cristal de 4 MHz

## Funcionamiento
El programa controla la secuencia típica de un semáforo mediante retardos de tiempo (`delay_ms`)
1. **LED 1 (PIN_C0)** encendido durante 5 segundos
2. **LED 3 (PIN_C6)** encendido durante 5 segundos
3. **LED 2 (PIN_C3)** encendido (como precaución/amarillo) durante 2 segundos
4. El ciclo se repite de manera infinita dentro de un bucle `while(TRUE)`

## Estructura del proyecto
* `Semaforo 3 LED.c`: Código fuente principal con la configuración de fuses, puertos y la lógica de secuencia

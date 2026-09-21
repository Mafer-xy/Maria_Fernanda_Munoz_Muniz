---
titulo: "Sesión 3 — como utilize un arduino"
fecha: 2026-09-04
autor: "María Fernanda Muñoz Muñiz"
equipo: "Fernanda Muñoz y Mario Osorio"
estado: borrador #borrador | completa 
---

# Sesión 3 - Como utilize un arduino

## Qué debía lograr hoy   

- [✅] Configurar el entorno de desarrollo del ESP32
- [✅] Controlar entradas y salidas digitales (LED, botón con pull-up y antirrebote)
- [✅] Establecer comunicación Bluetooth con un protocolo de comandos — la base del cerebro y el control remoto de tu carro.


## Qué usé

**Materiales**

- Tarjeta: ESP32 DevKit V1 (WROOM-32). Importante: debe ser ESP32 “clásico”; las variantes S3/C3 no tienen Bluetooth Classic y los ejemplos de BluetoothSerial no compilan en ellas.
- Cable: USB de datos.
- Breadboard: + jumpers.
- LED: 1 + 1 resistor 220 Ω.
- Botón: 1 (push button).
- Resistor: (Opcional) 1 10 kΩ si no usamos pull-up interno.

**Software:**

- Arduino IDE + Paquete de tarjetas ESP32.
- (Opcional) VS Code + Extensión Arduino.

## Qué hice y qué pasó (evidencia)

![arduino](../imgs/arduino.jpeg)

![1_0](../imgs/prendeapaga.jpeg)

![led](../imgs/1_0led.jpeg)

![rojoazul](../imgs/rojoazul.jpeg)

![rojoled](../imgs/rojoled.jpeg)
![azulled](../imgs/azulled.jpeg)

![print](../imgs/print.jpeg)
![println](../imgs/println.jpeg)

![boton](../imgs/botonrojoazul.jpeg)

![botonazul](../imgs/botonazul.jpeg)
![botonrojo](../imgs/botonrojo.jpeg)

![bluetooth](../imgs/oliverbaja.jg)
![Pie de foto: qué muestra esta imagen](img/sesionN_1.jpg)


## Qué falló y cómo lo resolví


-  ⁠*Síntoma:* El circuito fallaba y funcionada de manera diferente a la manera que se supone debia funcionar 
-  ⁠*Cómo lo encontré:* Al ver que el LED y el boton fucionaban de manera erronea revisamos cada conección del ESP32 y encontramos que en ciertas conecciones no generaba ninguna reacción
-  ⁠*Solución:* Cambiamos la conección de INPUT de un led y de esa manera se genero la reacción esperada de la programación

## Qué aprendí
3 a 5 líneas, con tus palabras. No es resumen del tema: es qué entendiste TÚ que antes no.!!!!!!!!!!!!!!!!

## Siguiente paso
Mejorar el uso del bluetooth y adaptarlo al movimiento de un motor




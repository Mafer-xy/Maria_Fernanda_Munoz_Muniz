---
titulo: "Sesión 5 — Mecanismos"
fecha: 2026-09-18
autor: "María Fernanda Muñoz Muñiz"
equipo: "Fernanda Muñoz y Mario Osorio"
estado: borrador #borrador | completa 
---

# Mecanismos

## Qué debía lograr hoy
 

- [✅] Entender cómo los mecanismos transforman el movimiento (velocidad ↔ par, rotación ↔ traslación, continuo ↔ intermitente)
- [✅] calcular relaciones de transmisión simples 
- [❌] Aplicarlo al tren motriz del carro — tocando mecanismos reales en un taller de estaciones.

## Qué usé

- Modelos impresos 3D de diferentes mecanismos:
    * Engrane Interno Helicoidal
    * Cónico Espiral
    * Espiral de Arquímedes
    * Reductor Cicloidal
    * Sinfín Multi-hilo + Corona
    * Engrane Intermitente
    * Cruz de Ginebra
    * Junta Carbán (Universal)
    * Obturador de láminas (leaf shutter)
    * Diferencial

## Qué hice y qué pasó (evidencia)

### Ejercicio: relación de transmisión

*Datos*

|Caso|	Motriz	|Conducido|	Datoconocido|
|:---:|:---:|:---:|:---:|
|A|	Z₁ = 5	|Z₂ = 10|	ω₂ = 10 rpm, τ₁ = 1 N·cm|
|B|	Z₃ = 5	|Z₄ = 20	|ω₃ = 20 rpm, τ₃ = 4 N·cm|

**Incógnitas:** ω₁ y τ₂ (caso A); ω₄ y τ₄ (caso B).

*Caso A*

i_A = Z₂ / Z₁ = 10 / 5 = **2**

ω₁ = i_A · ω₂ = 2 · 10 = **20 rpm**

τ₂ = i_A · τ₁ = 2 · 1 = **2 N·cm**

*Caso B*


i_B = Z₄ / Z₃ = 20 / 5 = **4**

ω₄ = ω₃ / i_B = 20 / 4 = **5 rpm**

τ₄ = i_B · τ₃ = 4 · 4 = **16 N·cm**

Resultados

|Caso|	i|	Velocidad|	Par|
|:---:|:---:|:---:|:---:|
|A|	2|	ω₁ = 20 rpm (entrada), ω₂ = 10 rpm (salida)|	τ₂ = 2 N·cm|
|B|	4|	ω₄ = 5 rpm|	τ₄ = 16 N·cm|

*Conclusión:* en ambos casos i > 1, así que el sistema reduce la velocidad y multiplica el par por el mismo factor.

### Tabla de engranajes

| Estación | ¿Qué transforma? (vel↔par, rot↔trasl, continuo↔intermitente, cambio de eje) | relación *i* estimada (cuenta dientes o vueltas) | ¿Reversible o autobloqueante? |¿Dónde lo has visto en la vida real?|¿Donde serviría en el carro o en un proyecto tuyo?|
|---:|:---:|:---:|:---:|:---:|:---:|
| A. Diferencial  | Transforma el movimiento rotatorio inicial y lo translada a cualquiera de las dos salidas segun se decida | aproximadamente 3.5 vueltas del piñon a 1 vuelta de la corona | Reversible | En los vehiculos funcionando para realizar vueltas | En la parte trasera de nuestro carro para realizar eso cambios de dirección |
| B. Cicloidal | Transforma una velocidad y bajo par a una velocidad baja con par alto | de 40-100 a 1 dependiendo del reductor | casi Autobloqueante | En reductores de velosidad de brazos roboticos industriales | En el movimiento de algun brazo robotico | 
| C. Cardán | Transmite rotación entre ejes que forman un ángulo | 1 a 1 | Reversible | En la flecha de transmisión de camionetas | transmitiendo potencia por los ejes del prototipo de un vehiculo |
| D. Obturador | Transforma un movimiento de rotación en uno de desplazamiento | Varia segun su diseño y su cantidad de varillas | Suele ser autobloqueante | En los lentes de las camaras | En compuertas de ventilación |
| E1. Cremallera | Transforma el movimiento de rotación a uno de translación | no niene. comparacion ya que se vuelve recto | Reversible | En el area de movimiento de la impresora ayudando a distribuir la tinta | Si se desea realisar una impresora |
| E1. Ginebra | transforma el movimiento de rotación continua a una intermitente | 6 a 1 | Autobloqueante | Personalmente no lo he visto, pero se solia utilizar en los proyectores de cine tradicionales. Se encargaban de la reproducción de la pelicula | Para realizar cambios de pagina o de imagen en una proyección |
| E2. Espiral | Cambia el eje realizando un giro 90 grados | aprox. 3 a 1 | Reversible | En taladros angulares | puede usarse para el eje trasero de los vehiculos |
| E2. Sinfín multi-hilo + corona | Reduce la velocidad y cambia los ejes de manera perpendicular | suele se de 20 a 1 | auto bloqueante | Afinadores de guitarra | si se desea construir una guitarra para el area de tención de cuerdas |

## Qué falló y cómo lo resolví

- **Síntoma:** En los calculos de velocidad de engranaje me daba una velocidad mayor a la del resultado
- **Cómo lo encontré:** Al momento de sacar la velocidad que daria el engranaje que estabamos calculando me daba una mayor a la del profesor 
- **Solución:** Me explicaron que la fuerza se toma en cuenta desde el centro del engranaje y entre mas se aleja del centro se necesita cada vez mas fuerza, por eso la velocidad disminuye

## Qué aprendí
Aprendí que existe una gran variedad de mecanismos los cuales se pueden utilizar en lugares donde nunca los pensarias y el como estas pueden cambiar ejes, ser intermitentes o como se transladan dependiendo de su rotación.
Tambien aprendi las formulas y los conceptos de transformación de velocidades de rotación tomando en cuenta la velocidad, los dientes, etc.
## Siguiente paso
Analizar cada engranaje y encontrar los mas optimos para realizar los carros del proyecto final
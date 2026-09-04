---
title: Programación, IA y Robótica 1
tags:
  - piar1
  - informatica
description: Índice PIAR1. Se describe el contenido de las Situaciones de Aprendizaje y su temporalización.
fecha-creación: 04/09/2026
otra: ñlsfklsdkf
---
![[recursos/PIAR1 SdAs.excalidraw.light.svg]]
# 🚀 Programación, IA y Robótica 1 

> **Marco de trabajo:** Misiones ágiles quincenales (4 sesiones de 55 min por misión) orientadas a la resolución de micro-retos prácticos y desarrollo colaborativo.
> **Acceso rápido:** [[./00_Guia_y_Evaluacion/sesion-0-presentacion|sesion-0-presentacion]]
> [[01_Materias/piar1/00_Guia_y_Evaluacion/sesion-0-presentacion]]


```python
# Algoritmo de comprobación de sensores
def verificar_sensor(distancia_cm: float) -> str:
    umbral_seguridad = 15.0  # cm
    if distancia_cm < umbral_seguridad:
        return "ALERTA: Obstáculo cercano"
    return "Camino despejado"

lecturas = [25.4, 18.2, 12.0, 5.5]
for medida in lecturas:
    estado = verificar_sensor(medida)
    print(f"Distancia: {medida} cm -> {estado}")
```

```c
#include <stdio.h>
#include <stdbool.h>

#define UMBRAL_SEGURIDAD 15.0

// Función para validar la distancia medida por el sensor
bool detectar_obstaculo(float distancia_cm) {
    return distancia_cm < UMBRAL_SEGURIDAD;
}

int main(void) {
    float lecturas[] = {25.4f, 18.2f, 12.0f, 5.5f};
    int total_lecturas = sizeof(lecturas) / sizeof(lecturas[0]);

    for (int i = 0; i < total_lecturas; i++) {
        if (detectar_obstaculo(lecturas[i])) {
            printf("[ALERTA] Obstaculo a %.2f cm\n", lecturas[i]);
        } else {
            printf("[OK] Distancia segura: %.2f cm\n", lecturas[i]);
        }
    }
    return 0;
}
```
---

## 🗺️ Mapa de Situaciones de Aprendizaje (SdA)

### 🕹️ SdA 1: Arcade Retro Lab — Videojuegos 2D con Scratch
* **Misión 1.1:** Guion técnico, personajes y movimiento cartesiano.
* **Misión 1.2:** Físicas de salto, gravedad y colisión con plataformas.
* **Misión 1.3:** Patrullas enemigas, obstáculos y clonación.
* **Misión 1.4:** Variables de marcador: vidas, puntuación y niveles.
* **Misión 1.5:** Pulido sonoro, estética y licencias Creative Commons.
* **Misión 1.6:** Gran Gala Arcade y torneo de evaluación inter-grupos.

### 🤖 SdA 2: Guardianes Digitales — Inteligencia Artificial Ética
* **Misión 2.1:** ¿Cómo piensan las máquinas? Aprendizaje humano vs. artificial.
* **Misión 2.2:** Entrenamiento de clasificadores en Machine Learning for Kids / Teachable Machine.
* **Misión 2.3:** Integración del modelo en Scratch: El Asistente Verde de reciclaje.
* **Misión 2.4:** Detectives de sesgos: discriminación algorítmica y equidad.
* **Misión 2.5:** Accesibilidad y síntesis de voz en asistentes virtuales.
* **Misión 2.6:** Festival de Asistentes Virtuales y premios de innovación.

### 🚜 SdA 3: Misión Rover — Robótica Móvil con BBC micro:bit
* **Misión 3.1:** Anatomía de micro:bit y programación en MakeCode.
* **Misión 3.2:** Ensamblaje del chasis 2WD y control de motores DC.
* **Misión 3.3:** Sensor de distancia por ultrasonidos y evasión de obstáculos.
* **Misión 3.4:** Sensores infrarrojos de suelo y seguimiento de línea negra.
* **Misión 3.5:** Reto integrador del laberinto mixto.
* **Misión 3.6:** Gran Torneo de Rovers y gala final de robótica.

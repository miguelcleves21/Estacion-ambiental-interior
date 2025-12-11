# Estación Ambiental Interior  
Proyecto para la materia **Sistemas Embebidos**  
Autor: **Miguel Ángel Cleves Bolívar**

La Estación Ambiental Interior es un proyecto orientado al diseño de un sistema embebido capaz de monitorear la calidad del aire en espacios cerrados mediante la tarjeta LicheeRV Nano. El sistema propone integrar sensores de CO₂, temperatura, humedad y material particulado, permitiendo obtener información confiable sobre las condiciones ambientales para favorecer entornos más seguros y saludables.

---

## Descripción del Proyecto

Este repositorio contiene el **planteamiento técnico** de una estación ambiental interior basada en la tarjeta **LicheeRV Nano**, enfocada en la medición de variables de calidad del aire en espacios cerrados.

El proyecto propone la integración de los siguientes sensores:

- **SCD41** – Medición de CO₂  
- **DHT22** – Temperatura y humedad  
- **GP2Y1010AU0F** – Material particulado PM2.5  
- **ADS1115** – Conversión analógica–digital de 16 bits

La documentación incluida corresponde a la **Entrega 1** del modelo CDIO (Concebir y Diseñar).

---
## Situación actual.

En espacios interiores como hogares, oficinas y aulas, la calidad del aire suele deteriorarse sin que las personas lo noten. Concentraciones elevadas de CO₂, humedad inadecuada o acumulación de polvo afectan la atención, el bienestar y la salud.

A pesar de su importancia, la mayoría de lugares no cuentan con sistemas de monitoreo continuo, y los dispositivos comerciales disponibles son costosos o no ofrecen acceso a los datos ni posibilidad de personalización.

---
## Problema a tratar

Actualmente no existe un sistema accesible, abierto y de bajo costo que permita monitorear en tiempo real variables críticas de calidad de aire interior como CO₂, temperatura, humedad y partículas en suspensión.

Sin esta información, es difícil detectar condiciones inadecuadas, tomar decisiones de ventilación o identificar ambientes que puedan afectar la salud y el bienestar de las personas.

---
## Justificacion

El monitoreo ambiental interior es fundamental para prevenir problemas de salud, mejorar el confort y optimizar la ventilación en espacios cerrados.

Un sistema propio, basado en hardware abierto y de bajo costo, permite acceder a datos reales, personalizar funciones y desarrollar soluciones adaptadas al contexto local.

---

## Objetivo General

Diseñar e implementar una estación ambiental interior basada en la LicheeRV Nano que permita medir CO₂, temperatura, humedad y partículas en suspensión, generando datos confiables para apoyar la toma de decisiones sobre la calidad del aire.

---

## Objetivos Específicos

- Integrar los sensores a la tarjeta de desarrollo mediante interfaces digitales y un ADC externo.
- Realizar la adquisición y procesamiento básico de las señales para obtener mediciones confiables de CO₂, temperatura, humedad y partículas.
- Implementar un módulo o servicio que permita leer, registrar y exponer los datos.
- Desarrollar una interfaz simple para visualizar las mediciones de calidad de aire.

---

## Hardware

###SCD41 Sensor de CO₂

El sensor SCD41 es un módulo avanzado basado en tecnología fotoacústica que permite medir concentraciones de CO₂ con alta precisión y estabilidad a largo plazo. Su diseño compacto y su integración digital mediante interfaz I²C lo convierten en una solución ideal para sistemas embebidos orientados al monitoreo ambiental. Gracias a su capacidad para entregar mediciones confiables incluso en ambientes dinámicos, el SCD41 permite evaluar la calidad del aire en interiores y detectar niveles potencialmente perjudiciales para la salud o el rendimiento humano

### DHT22 Sensor de Temperatura y Humedad

El DHT22 es un sensor capacitivo que ofrece mediciones digitales de temperatura y humedad con buena precisión y estabilidad, lo que lo hace adecuado para aplicaciones de monitoreo ambiental en interiores. Su interfaz de comunicación es sencilla y su respuesta es suficientemente rápida para capturar cambios típicos en el entorno. Al complementar las mediciones de CO₂, el DHT22 permite contextualizar las condiciones térmicas del espacio y relacionarlas con el confort ambiental y la circulación de aire.

### GP2Y1010AU0F Sensor de material particulado PM2.5

El GP2Y1010AU0F es un sensor óptico de dispersión de luz diseñado para detectar la concentración de polvo fino y partículas suspendidas en el aire, incluyendo PM2.5. Funciona mediante un diodo LED infrarrojo y un fototransistor que detecta la cantidad de luz reflejada por las partículas presentes en la cámara interna. Esta técnica ofrece buen rendimiento para estimar la calidad del aire en interiores, especialmente en presencia de humo, polvo u otras fuentes contaminantes. Su naturaleza analógica requiere acondicionamiento y conversión para integrarlo en sistemas digitales.

### ADS1115 Convertidor Análogo a Digital (ADC) de 16 bits

El ADS1115 es un ADC externo de alta precisión que proporciona conversión analógica-digital de 16 bits, lo cual mejora significativamente la resolución comparado con conversores integrados de microcontroladores típicos. Su interfaz I²C y sus canales de entrada multipropósito permiten digitalizar señales provenientes de sensores como el GP2Y1010AU0F con gran detalle y estabilidad. Incorporar el ADS1115 garantiza que las mediciones del sensor de partículas sean consistentes, evitando ruidos o imprecisiones que comprometan el análisis ambiental.

---



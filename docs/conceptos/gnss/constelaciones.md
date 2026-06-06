# Constelaciones GNSS y Sistemas de Corrección

## ¿Qué es una constelación GNSS?

Una constelación GNSS (Global Navigation Satellite System) es un conjunto de satélites que transmite señales de posicionamiento a receptores terrestres.

Mientras más satélites pueda utilizar un receptor, generalmente se obtiene:

- Mayor disponibilidad de señal.
- Mejor precisión.
- Menor tiempo para obtener una solución RTK.
- Mejor desempeño en zonas urbanas, bosques o terrenos con obstrucciones.

En condiciones ideales, la precisión final depende además de la calidad del receptor, las correcciones utilizadas y el entorno de medición.

---

## Principales constelaciones GNSS
| Constelación | País / Organización | Estado             |
| ------------ | ------------------- | ------------------ |
| GPS          | Estados Unidos      | Operativa          |
| GLONASS      | Rusia               | Operativa          |
| Galileo      | Unión Europea       | Operativa          |
| BeiDou       | China               | Operativa          |
| NavIC        | India               | Cobertura regional |

---

### GPS

El sistema GNSS más utilizado a nivel mundial.

Recomendación: Imprescindible para cualquier receptor moderno. Se encuentra presente en todos los receptores GNSS Trimble.

### GLONASS

Sistema desarrollado por Rusia.

Aporta satélites adicionales que mejoran la disponibilidad de señal y la continuidad de la solución GNSS.

Recomendación: Muy útil en levantamientos con obstrucciones.

### Galileo

Sistema desarrollado por la Unión Europea.

Ofrece señales modernas, excelente disponibilidad y una alta calidad de servicio. Actualmente es una de las constelaciones más valoradas para aplicaciones topográficas y geodésicas.

Recomendación: Prioritaria junto con GPS.

### BeiDou

Sistema desarrollado por China.

Posee una gran cantidad de satélites operativos y contribuye significativamente a mejorar la disponibilidad y robustez de las soluciones RTK.

Recomendación: Muy recomendable para aumentar disponibilidad y confiabilidad en terreno.

### NavIC

Sistema desarrollado por India.

Su cobertura principal está orientada al territorio indio y regiones cercanas.

Recomendación: Poco relevante para operaciones en Chile y Latinoamérica.

---

## Sistemas de Corrección y Aumentación

Las constelaciones entregan la posición base, pero existen sistemas complementarios que permiten mejorar la precisión.

### QZSS

QZSS (Quasi-Zenith Satellite System) es un sistema japonés diseñado para complementar GPS.

Cobertura aproximada:

- Japón
- Corea
- Australia
- Parte del Pacífico Occidental

Puede proporcionar servicios de corrección de alta precisión para usuarios dentro de su área de cobertura.

Relevancia para Chile: No aplica.

### SBAS

SBAS (Satellite-Based Augmentation System) es una familia de sistemas que transmiten correcciones diferenciales para mejorar la precisión GNSS.

Normalmente permiten precisiones del orden de:

- 1 a 2 metros horizontales.
- Mejor integridad y confiabilidad de la solución.

### Sistemas SBAS existentes

| Sistema | Región                        |
| ------- | ----------------------------- |
| WAAS    | Norteamérica                  |
| EGNOS   | Europa                        |
| MSAS    | Japón                         |
| GAGAN   | India                         |
| SDCM    | Rusia                         |
| SACCSA  | Sudamérica (alcance limitado) |

---

## ¿Qué constelaciones son importantes para cotizaciones en Chile?

Para aplicaciones topográficas y geoespaciales en Chile, se recomienda que el receptor soporte las siguientes constelaciones:

- GPS
- Galileo
- BeiDou
- GLONASS

Un receptor que soporte GPS + Galileo + BeiDou + GLONASS tendrá un desempeño significativamente mejor que uno que utilice únicamente GPS.

En la práctica, para equipos topográficos modernos, la presencia de las cuatro constelaciones globales principales (GPS, Galileo, BeiDou y GLONASS) es actualmente el estándar esperado.
---
title: Teoría de la Información de Shannon / Entropía
aliases: [Entropía de Shannon, Teoría de la Información]
tags: [principio, información, entropía, ciencias-de-la-computación]
domain: Sistemas-Formales
subdomain: Teoría-de-la-Información
authors: [Claude Shannon]
year: 1948
status: stable
related: [Segundo-Principio-de-la-Termodinámica]
---

# Teoría de la Información de Shannon (Entropía de la Información)

## Definición en una frase
> La información puede cuantificarse; la entropía de un mensaje mide la incertidumbre media o el número mínimo de bits necesarios para codificarlo, estableciendo límites fundamentales a la compresión y a la comunicación fiable.

## Explicación completa
Claude Shannon definió la entropía de una variable aleatoria discreta \( X \) como \( H(X) = -\sum p(x) \log_2 p(x) \). Esta cantidad es el contenido medio de información por símbolo y el límite inferior del número medio de bits necesarios para codificar mensajes de esa fuente. Los teoremas de capacidad de canal dan la tasa máxima a la que se puede transmitir información de forma fiable a través de un canal ruidoso. La teoría creó el fundamento matemático de toda la comunicación digital, la compresión de datos y la codificación.

## Explicación al estilo Feynman
Imagina que quieres enviar un mensaje con el menor número posible de preguntas de sí/no (bits). Si el mensaje es completamente predecible, necesitas casi ningún bit. Si es completamente sorprendente, necesitas muchos. La entropía de Shannon te dice exactamente cuántos bits, en promedio, se requieren. También te dice cuánto ruido puedes tolerar antes de que el mensaje se vuelva irrecuperable.

## Metáforas y analogías clave

1. **“Vng mñn”** — Eliminar las vocales comprime el mensaje; el contexto (redundancia) todavía permite recuperarlo.
2. **Diccionario de palabras esperadas** — Los mensajes comunes reciben códigos cortos; los raros reciben códigos largos (como la codificación de Huffman).
3. **Medidor de sorpresa** — Cuanto más sorprendente es un evento, más información lleva.

## Ejemplos concretos

1. **Compresión de datos** — ZIP, JPEG, MP3 se acercan (pero no pueden superar) el límite de entropía de la fuente.
2. **Códigos de corrección de errores** — El teorema de codificación de canal de Shannon explica por qué podemos enviar datos casi sin errores si nos mantenemos por debajo de la capacidad del canal (usado en comunicación espacial profunda, 5G, etc.).
3. **Lengua inglesa** — La entropía del inglés escrito es aproximadamente 1–1,5 bits por carácter debido a su alta redundancia.

## Anclas cuantitativas / de datos
- Entropía: \( H(X) = -\sum p_i \log_2 p_i \)
- Función de entropía binaria para una moneda justa: 1 bit
- Capacidad de canal de un canal ruidoso: \( C = B \log_2 (1 + S/N) \) (Shannon-Hartley)

## Contexto histórico y de descubrimiento
El artículo de Shannon de 1948 “A Mathematical Theory of Communication” fundó el campo. Estuvo motivado por problemas en los Laboratorios Bell sobre la transmisión de información a través de líneas telefónicas ruidosas.

## Relaciones

### Se basa en / presupone
- Teoría de la probabilidad
- Concepto de información como reducción de incertidumbre

### Influye / conduce a
- Toda la comunicación y almacenamiento digital modernos
- Analogía formal profunda con la entropía termodinámica
- Aprendizaje automático (pérdida de entropía cruzada, etc.)

### Contrasta con
- Teorías semánticas de la información (Shannon ignoró deliberadamente el significado)

## Conceptos erróneos comunes
- “La teoría de la información trata del significado de los mensajes.” → La teoría de Shannon trata de las propiedades estadísticas de las señales, no de la semántica.
- “Puedes comprimir cualquier archivo arbitrariamente.” → La compresión sin pérdida no puede ir por debajo de la entropía de la fuente en promedio.

## Ver también
- [Segundo Principio de la Termodinámica](../../../Science/Physics/Thermodynamics/Second-Law-of-Thermodynamics.md) (vínculos matemáticos y conceptuales profundos)

## Tags
#principio #teoría-de-la-información #entropía #shannon #compresión #comunicación

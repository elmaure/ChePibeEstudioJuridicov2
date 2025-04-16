# ChePibeEstudioJuridicov2
Version final para CODERHOUSE

Generador de Demandas - Versión Actualizada
Este proyecto está basado en la primera entrega del curso de Coder House. Partimos de esa base y trabajamos sobre la misma entrega para mejorarla, corrigiendo problemas y ampliando sus capacidades.

Objetivo de esta versión
El objetivo principal de esta actualización fue mejorar el prompt utilizado, ya que en la versión anterior nos encontramos con limitaciones importantes al momento de generar textos jurídicos extensos. En particular, el caso de uso elegido para esta entrega fue la redacción de una demanda de amparo por mora, un escrito que, si bien es considerado "escueto" dentro del ámbito jurídico, requiere varias carillas y una redacción completa, precisa y formal.

Problemas detectados
Durante las pruebas, nos enfrentamos a múltiples inconvenientes con la IA (ChatGPT) al intentar generar este tipo de documentos:

La IA tiende a resumir automáticamente los textos, incluso cuando se le solicita explícitamente que no lo haga.

Modifica el texto original del modelo jurídico, alterando su estructura o lenguaje, lo cual no es aceptable cuando se parte de un escrito base que debe mantenerse casi sin cambios.

Suele interrumpir los textos largos con puntos suspensivos, paréntesis o aclaraciones innecesarias.

A pesar de usar prompts negativos y dar ejemplos de cómo debía redactar, los errores persistían.

Solución implementada
La estrategia que permitió resolver esta situación fue diseñar un nuevo prompt que divide la respuesta en múltiples partes. De este modo, la IA queda esperando que el usuario ingrese la palabra “siguiente” para continuar generando el texto, párrafo por párrafo, sin alterar la redacción del modelo.

Este enfoque nos permitió:

Controlar mejor la longitud de la respuesta.

Evitar resúmenes o cortes inesperados.

Conservar fielmente la estructura del modelo original.

Reemplazar únicamente los datos esenciales (nombres, juzgado, expediente, etc.).

Al finalizar el proceso, todas las partes generadas se consolidan en un documento Word completo, listo para ser utilizado.

Implementación
No utilice Google Colab para hacer la implementacion sino que este prompt fue inserto directamente en ChatGPT mediante la creación de un GPT personalizado.

👉 Podés probar el GPT en el siguiente enlace: https://chatgpt.com/g/g-67eb08f7cbb88191909c05479bdef102-amparoxmora

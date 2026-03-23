# Práctica de chino

Sitio estático de tarjetas de estudio para practicar vocabulario y caracteres chinos, inspirado en una dinámica similar a AnkiWeb.

## Funcionalidades

- Selección de una o varias lecciones
- Visualización de tarjetas con hanzi
- Revelado de pinyin, significado y oración de ejemplo
- Marcado de tarjetas como:
  - **La sabía**
  - **No la sabía**
- Lote automático de tarjetas **a repasar**
- Opción de repasar pendientes al finalizar
- Reinicio de ronda o de lección
- Guardado de progreso en `localStorage`

## Tecnologías

- HTML
- CSS
- JavaScript puro

No requiere backend ni base de datos.

## Estructura

Los datos de las tarjetas están embebidos dentro del mismo `index.html`, en un objeto `APP_DATA`, agrupado por lección.

Cada lección tiene esta estructura:

```js
{
  id: "leccion-1",
  title: "Lección 1",
  description: "Descripción",
  items: [
    {
      id: "l1-001",
      hanzi: "你",
      pinyin: "nǐ",
      meaning: "tú",
      example_hanzi: "你好。",
      example_pinyin: "Nǐ hǎo.",
      example_es: "Hola."
    }
  ]
}

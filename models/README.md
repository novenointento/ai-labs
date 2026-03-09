# Models

Esta carpeta documenta los modelos de IA utilizados en el laboratorio.

El objetivo no es almacenar modelos grandes en el repositorio, sino registrar:

* qué modelos se usan
* cómo se descargan
* cómo se configuran
* pruebas de rendimiento o calidad

Los modelos grandes (GGUF, safetensors, etc.) normalmente **no se almacenan directamente en Git**, sino que se descargan mediante scripts o herramientas externas.

## Contenido esperado

Ejemplos de contenido que puede aparecer aquí:

* scripts de descarga de modelos
* configuraciones de inferencia
* comparativas entre modelos
* documentación sobre cuantización
* instrucciones para ejecutar modelos locales

## Ejemplo de estructura

```
models
├─ README.md
├─ ollama_models.md
├─ model_comparisons.md
└─ download_scripts/
```

## Notas

Siempre que sea posible se intentará documentar:

* tamaño del modelo
* requisitos de hardware
* uso de memoria
* rendimiento aproximado

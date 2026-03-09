# Docker Environment

Esta carpeta contiene configuraciones Docker utilizadas para reproducir entornos de experimentación.

El objetivo es poder levantar rápidamente los servicios necesarios para realizar pruebas de IA.

## Posibles servicios

Ejemplos de componentes que pueden aparecer aquí:

* entornos de ejecución de LLM
* bases de datos vectoriales
* servicios auxiliares
* entornos de desarrollo

## Ejemplo de contenido

```
docker
├─ README.md
├─ docker-compose.yml
├─ ollama_stack/
└─ rag_stack/
```

## Objetivo

Facilitar la reproducción del laboratorio en diferentes máquinas mediante configuraciones de infraestructura como código.

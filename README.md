# Sistema de Control de Calidad Industrial

Sistema de control de calidad para una fábrica ficticia de piezas de precisión, desarrollado en Python con programación orientada a objetos. Trabajo práctico de **Estructuras de Datos y Programación** (ITBA, 2026).

Registra lotes de producción, toma muestras, asigna inspectores certificados y equipos calibrados, y ejecuta inspecciones visuales y dimensionales. Con los defectos encontrados decide si cada lote se aprueba o se rechaza, y prioriza los reportes según su gravedad.

## Características

- **Dominio:** `Empresa`, `Lote`, `Muestra`, `Inspeccion`, `Profesional`, `Equipo`, `Procedimiento`, `Reporte` y `Defecto`.
- **POO:** encapsulamiento con `@property`, clases abstractas (`ABC`), herencia simple, multinivel y múltiple, polimorfismo, composición y métodos especiales (`__eq__`, `__hash__`, `__iter__`, `__contains__`, `__lt__`).
- **Excepciones:** jerarquía propia de excepciones de dominio.
- **Estructuras de datos propias:** lista enlazada, pila, cola, árbol AVL (índices por fecha y búsqueda por rango) y max-heap como cola de prioridad.
- **Programación funcional:** `map`, `filter`, `reduce`, lambdas, generadores, `*args` y `**kwargs`.
- **Persistencia:** exportación de reportes a JSON y guardado/carga del estado completo con pickle.
- **Tests:** 521 tests automatizados con pytest.

## Tecnologías

Python 3, solo con la biblioteca estándar (`tkinter`, `datetime`, `uuid`, `abc`, `functools`, `random`). pytest para los tests.

## Cómo correrlo

```
py main.py          # demo por script
py consola.py       # menú por consola
py interfaz.py      # interfaz gráfica
py -m pytest        # tests
```

## Equipo

Trabajo práctico grupal. La lógica del sistema se desarrolló entre dos integrantes en conjunto; la interfaz gráfica estuvo a cargo de una tercera.

| Integrante | Aporte principal |
|---|---|
| Charles Tronchetti | Lógica de dominio y estructuras de datos (lista enlazada, pila, cola, árbol AVL, heap), jerarquía de clases y excepciones, serialización, demo y documentación |
| Martin Papaleo | Lógica de dominio y estructuras de datos (lista enlazada, pila, cola, árbol AVL, heap), jerarquía de clases y excepciones, serialización, demo y documentación |
| Martina Risso | Interfaz gráfica |

## Nota

Partes del código se desarrollaron con asistencia de IA (Claude) y fueron revisadas por el equipo.

## Licencia

Ver el archivo `LICENSE`
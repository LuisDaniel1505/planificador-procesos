# Planificador de Procesos

Aplicación web (un solo archivo HTML) para calcular la planificación de procesos de un sistema operativo y visualizar el diagrama de Gantt.

## Algoritmos soportados

| Algoritmo | Tipo | Regla |
|---|---|---|
| FCFS | No apropiativo | Orden de llegada |
| SJF / SJN | No apropiativo | Ráfaga más corta entre los que ya llegaron |
| Prioridad | No apropiativo | Mayor prioridad (orden configurable) |
| SRT / SRTF | Apropiativo | Menor tiempo restante |
| Round Robin | Apropiativo | Quantum fijo, cola circular |

## Cómo usar

1. Abre `planificador.html` en tu navegador (doble clic).
2. Elige el algoritmo y el número de procesos.
3. Genera los campos y captura el tiempo de llegada y la ráfaga de CPU (y prioridad o quantum si aplica).
4. Pulsa "Calcular y dibujar Gantt".

## Resultados

- Diagrama de Gantt en cuadrícula: ejecución, tiempo de espera ("TE") y cola de listos.
- Tabla con finalización, retorno (TAT) y espera por proceso, y sus promedios.

## Convenciones

- Los procesos se ordenan por **tiempo de llegada**.
- En **Prioridad**: "ascendente" = menor número es mayor prioridad; "descendente" = mayor número es mayor prioridad.
- El eje de tiempo inicia en 0 (borde izquierdo); cada celda se etiqueta con el tiempo en que termina.

# A1.1.b - Ejecución de un programa en ensamblador LC-3

Completa esta plantilla en tu repositorio individual creado al aceptar el
assignment de Classroom 50.

## Identificación

- **Nombre y apellidos:** [Tu nombre y apellidos]
- **Módulo:** Entornos de desarrollo (EDES)
- **Unidad:** U1 - Introducción al desarrollo de software
- **Práctica:** A1.1.b - Ejecución de un programa en ensamblador LC-3
- **Fecha:** [AAAA-MM-DD]
- **Simulador utilizado:** [LC3 Simulator / LC3web / otro]

## Enunciado y recursos

- **Enunciado:** https://revilofe.github.io/section3/u01/practica/EDES-U1.-Practica012/
- **Simulador:** [Enlace al simulador utilizado]

## 1. Código LC-3

Incluye aquí el código ensamblador utilizado. Conserva las etiquetas `NUM1`,
`NUM2` y `ASCII_ZERO` y documenta cualquier cambio que realices.

```asm
; Pega aquí el código LC-3 utilizado.
```

## 2. Seguimiento paso a paso

Anota el PC según la convención que utilices e indica los valores observados o
deducidos. Si un dato no aparece en el simulador, escribe `no visible` y explica
cómo has obtenido el valor esperado.

| Instrucción ejecutada | PC (antes -> después) | Registro o efecto | Valor observado |
|---|---|---|---|
| `LD R0, NUM1` | | `R0` | |
| `LD R1, NUM2` | | `R1` | |
| `ADD R2, R0, R1` | | `R2` | |
| `LD R3, ASCII_ZERO` | | `R3` | |
| `ADD R0, R2, R3` | | `R0` | |
| `TRAP x21` | | Salida | |
| `HALT` | | Estado de ejecución | |

### Resultado inicial

- **Valor numérico calculado:** [Valor]
- **Código ASCII obtenido:** [Valor hexadecimal]
- **Carácter mostrado:** [Carácter]

## 3. Respuestas sobre la ejecución

### 1.a. Ejecución del procesador

1. ¿Qué función cumple el PC?

   [Respuesta]

2. ¿Cómo ayuda el PC a seguir la secuencia de instrucciones?

   [Respuesta]

3. Explica las fases de búsqueda, decodificación y ejecución.

   [Respuesta]

4. ¿Qué observas directamente en el simulador?

   [Respuesta]

5. ¿Qué parte solo puedes inferir?

   [Respuesta]

### 1.b. Memoria y registros

1. `NUM1`: [Valor]
2. `NUM2`: [Valor]
3. `ASCII_ZERO`: [Valor y significado]
4. Datos almacenados en esas posiciones: [Respuesta]
5. Valores finales de `R0`, `R1`, `R2` y `R3`: [Respuesta]
6. Funcionamiento de `LD` y `ADD`: [Respuesta]

### 1.c. Comunicación con la salida

1. Función de `TRAP x21`: [Respuesta]
2. Relación entre `OUT` y la consola simulada: [Respuesta]
3. Motivo por el que no se utiliza el teclado: [Respuesta]

### 1.d. Recorrido de instrucciones y datos

[Describe el recorrido desde los valores de memoria hasta la suma, la
conversión a ASCII y la salida del carácter `8`. Explica el papel del
procesador, la memoria, los registros y la salida simulada.]

### 1.e. Relación entre LC-3 y C

[Compara el nivel de abstracción, la forma de expresar la operación, el uso de
registros y memoria, la salida y las herramientas necesarias.]

### 1.f. Límites del modelo

[Explica qué aspectos de un procesador, la memoria y la entrada/salida reales
no reproduce el simulador LC-3 y diferencia la consola simulada de un
periférico físico.]

## 4. Modificación de datos y predicción

Cambia los datos para operar con `2` y `6`.

- **Cambios realizados en `.FILL`:** [Explicación]
- **Predicción para `R2`:** [Valor]
- **Predicción para `R0`:** [Valor hexadecimal]
- **Predicción del carácter:** [Carácter]
- **Resultado observado tras ejecutar:** [Comparación con la predicción]

## 5. Comparación con C

Incluye un ejemplo equivalente en C y completa la comparación.

```c
/* Pega aquí el ejemplo equivalente en C. */
```

| Aspecto | LC-3 | C |
|---|---|---|
| Nivel de abstracción | | |
| Forma de expresar la suma | | |
| Uso visible de registros y memoria | | |
| Mecanismo de salida | | |
| Herramienta necesaria | | |

## 6. Evidencias

Incluye una captura donde se vean la consola con el resultado `8` y, si es
posible, el estado del simulador.

![Consola del simulador mostrando el resultado 8](ruta/a/la/captura.png)

## 7. Reflexión final

[Explica qué has aprendido sobre la relación entre instrucciones, PC,
registros, memoria, procesador y salida, y sobre los límites de un modelo
simulado.]

## 8. Comprobación de la entrega

- [ ] El código LC-3 se ensambla sin errores.
- [ ] La tabla recoge el seguimiento de las instrucciones.
- [ ] Se distingue `x0008` del código ASCII `x0038`.
- [ ] La consola muestra el carácter `8`.
- [ ] Se ha probado la modificación con los valores `2` y `6`.
- [ ] Se han respondido los apartados 1.a a 1.f.
- [ ] Se ha incluido la comparación con C.
- [ ] Se ha añadido la captura y la reflexión final.
- [ ] Se han sustituido todos los marcadores entre corchetes.

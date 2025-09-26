# Parcial de Programación I (Java) — Versión A

> **Duración:** 90 minutos
> **Lenguaje:** Java (JDK 17+)
> **Modalidad:** Individual, sin internet ni IA
> **Ejecución:** Por consola

---

## Instrucciones generales

* Usa `Scanner` para leer desde teclado.
* Valida entradas **numéricas** y controla la **división por cero** cuando aplique.
* Imprime exactamente lo solicitado; cuida mayúsculas, espacios y saltos de línea.
* Entrega un proyecto con la siguiente estructura:

```
/Codigo_ApellidoNombre/
  src/
    Ejercicio1.java
    Ejercicio2.java
    Ejercicio3.java   (opcional)

```

**Puntaje:**

* Ejercicio 1 (35 pts)
* Ejercicio 2 (35 pts)
* Ejercicio 3 opcional (hasta +10 pts)
* Estilo/validaciones (20 pts)

**Criterios de calificación (resumen):** Correctitud (60%), validaciones (15%), claridad/estilo (15%), pruebas mínimas mostradas en consola (10%).

---

## Ejercicio 1 (35 pts)

**Enunciado**
Solicita **dos números reales** `a` y `b`.

* Si `a > b`: muestra la **suma** (`a + b`) y la **diferencia** (`a - b`).
* En caso contrario (incluye `a == b`): muestra el **producto** (`a * b`) y la **división** (`a / b`, del **primero respecto al segundo**).
* Si debes dividir y `b == 0`, imprime: `Division no definida (b es 0)` y **no** intentes la división.

**Ejemplos de ejecución:**

```
Entrada:
a=8.5
b=3
Salida:
Suma: 11.5
Diferencia: 5.5
```

```
Entrada:
a=3
b=6
Salida:
Producto: 18.0
Division (a/b): 0.5
```

---

## Ejercicio 2 (35 pts)

**Enunciado**
Pide **tres notas** `n1`, `n2`, `n3` en escala **0.0–5.0**. Calcula el **promedio** con dos decimales y muestra:

* `Promocionado` si **promedio ≥ 4.5**
* `Regular` si **4.0 ≤ promedio < 4.5**
* `Reprobado` si **promedio < 4.0**

**Validación:** cada nota debe estar en `[0.0, 5.0]`. Si alguna no lo está, imprime `Nota invalida` y **termina** el ejercicio.

**Ejemplo:**

```
Entrada:
4.8, 4.2, 5.0
Salida:
Promedio: 4.67
Estado: Promocionado
```

**Sugerencia de formato (opcional):**

```java
System.out.printf("Promedio: %.2f%n", promedio);
```

---

## Ejercicio 3 — Opcional (+10 pts)

**Enunciado**
Declara tres vectores `vector1`, `vector2`, `vector3` de **cinco enteros** cada uno.

* Pide 5 valores para `vector1` y 5 para `vector2`.
* Calcula `vector3[i] = vector1[i] + vector2[i]`.
* Muestra los tres vectores en **una línea cada uno**.

**Ejemplo:**

```
vector1: 1 2 3 4 5
vector2: 5 4 3 2 1
vector3: 6 6 6 6 6
```

**Sugerencia (lectura de arreglos):**

```java
int[] v = new int[5];
for (int i = 0; i < 5; i++) v[i] = sc.nextInt();
```

---

## Casos de prueba mínimos recomendados

* **Ej1:** casos `a > b`, `a < b`, `a == b`, y división con `b = 0`.
* **Ej2:** valores en los límites (0.0 y 5.0), una nota fuera de rango, y un caso para cada categoría.
* **Ej3 (opcional):** vectores con positivos, negativos y ceros.

---

## Buenas prácticas esperadas

* Nombres descriptivos (`promedio`, `vector1`, `estado`).
* Mensajes de salida claros y consistentes con los ejemplos.
* Comentarios **breves** sobre bloques no triviales.

---

¡Éxitos! ✨

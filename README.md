# Tarea Final - Árbol Binario de Búsqueda (BST)

## Información 

- **Estudiante:** Lester Payes 0905-24-22750
- **Curso:** Programación 3
- **Lenguaje:** Java 17
- **IDE utilizado:** Eclipse IDE
- **Repositorio:** GitHub

---

# Objetivo

El objetivo de esta práctica fue implementar y analizar un Árbol Binario de Búsqueda (BST), aplicando conceptos de recursividad, recorridos, validación de estructuras y manipulación de árboles.

Además de las operaciones básicas del BST, se desarrollaron cinco problemas obligatorios y cuatro ejercicios extra para reforzar el aprendizaje de estructuras de datos.

---

# Compilación y ejecución

## Desde Eclipse

1. Importar el proyecto Maven.
2. Abrir la clase `Principal.java`.
3. Ejecutar:

```text
Run As → Java Application
```

## Desde consola

Compilar:

```bash
mvn clean compile
```

Ejecutar:

```bash
mvn exec:java -Dexec.mainClass="umg.edu.progra.arboles.Principal"
```

---

# Problema 1 - Conteo total de nodos

## Método implementado

```java
public int contarNodos()
```

## Explicación

Este método cuenta todos los nodos existentes en el árbol utilizando recursividad. La idea es visitar cada nodo y sumar:

- El nodo actual.
- Los nodos del subárbol izquierdo.
- Los nodos del subárbol derecho.

## Ejemplo

### Resultado

```text
Tamanio: 8
Contar nodos (recursivo): 8
```

---

# Problema 2 - Verificar balanceo

## Método implementado

```java
public boolean esBalanceado()
```

## Explicación

Permite determinar si el árbol está balanceado. Se considera balanceado cuando la diferencia entre la altura del subárbol izquierdo y derecho no supera una unidad.

## Resultado obtenido

```text
Arbol principal balanceado?: true
Arbol desbalanceado balanceado?: false
```

---

# Problema 3 - Validación de BST

## Método implementado

```java
public boolean esBSTValido()
```

## Explicación

Comprueba que el árbol respete las reglas de un BST:

```text
Izquierda < Raíz < Derecha
```

en todos los niveles del árbol.

## Resultado obtenido

```text
Arbol principal es BST valido?: true
Arbol roto es BST valido?: false
```

---

# Problema 4 - Ancestro Común Más Bajo

## Método implementado

```java
public int ancestroComunMasBajo(int a, int b)
```

## Explicación

Busca el primer nodo que actúa como ancestro común de dos valores dentro del árbol.

## Ejemplos

```text
LCA(10,40) = 30
LCA(10,80) = 50
LCA(60,80) = 70
```

---

# Problema 5 - Invertir árbol

## Método implementado

```java
public void invertir()
```

## Explicación

Convierte el árbol en su versión espejo intercambiando los hijos izquierdo y derecho de cada nodo.

## Resultado obtenido

### Antes

```text
10 20 30 40 50 60 70 80
```

### Después

```text
80 70 60 50 40 30 20 10
```

---

# Ejercicio Extra E1 - K-ésimo menor

## Método implementado

```java
public int kEsimoMenor(int k)
```

## Explicación

Obtiene el elemento ubicado en una posición específica del recorrido InOrden.

## Resultados

```text
k=1 -> 10
k=3 -> 30
k=5 -> 50
k=8 -> 80
```

---

# Ejercicio Extra E2 - Impresión por rango

## Método implementado

```java
public void imprimirRangoOrdenado(int min, int max)
```

## Explicación

Muestra únicamente los valores que se encuentran dentro de un intervalo definido.

## Resultado

```text
20 30 40 50 60
```

---

# Ejercicio Extra E3 - Diámetro del árbol

## Método implementado

```java
public int diametro()
```

## Explicación

Calcula la longitud del camino más largo que puede recorrerse entre dos nodos del árbol.

## Resultado

```text
Diametro del arbol: 5
```

---

# Ejercicio Extra E4 - Construcción desde argumentos

## Explicación

Permite crear un BST utilizando valores enviados mediante argumentos al ejecutar el programa.

## Ejemplo de ejecución

```text
45 25 70 10 30 60 90
```

## Resultado

```text
Valores ordenados:
10 25 30 45 60 70 90
```

---

# Aprendizajes obtenidos

Durante el desarrollo de esta práctica reforcé el uso de recursividad en árboles binarios, comprendí mejor el funcionamiento interno de un BST y practiqué algoritmos relacionados con recorridos, validaciones estructurales y análisis de nodos.

También aprendí a trabajar con Git y GitHub utilizando commits progresivos para documentar cada avance realizado durante la implementación.

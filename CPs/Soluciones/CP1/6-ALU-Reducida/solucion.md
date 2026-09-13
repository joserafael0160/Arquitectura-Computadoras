# CP1 - Ejercicio 6: ALU Reducida

## 📋 Enunciado
Implementar en Logisim un circuito que, dado dos números de 4 bits y un selector para escoger la operación a realizar, dé como salida el resultado de operar ambos números según la operación seleccionada. Las operaciones a incluir son: suma (`00`), resta (`01`), and (`10`), y or (`11`).

TIP: Este circuito se conoce como Unidad Aritmética Lógica (ALU), que es donde se realizan las operaciones básicas en un microprocesador.

## 💡 Solución
Entradas: `A[3:0]`, `B[3:0]` (4 bits cada una), `Sel[1:0]` (2 bits).  
Salida: `Result[3:0]` (4 bits).

| Sel | Operación |
| :---: | :--- |
| 00 | Suma (`A + B`) |
| 01 | Resta (`A - B`) |
| 10 | AND (`A ∧ B`) |
| 11 | OR (`A ∨ B`) |


Decidí reutilizar los subcircuitos `Sumador 4 bits` y `Restador 4 bits` de los ejercicios anteriores, junto con compuertas AND y OR configuradas a 4 bits de ancho. Las cuatro operaciones se calculan en paralelo y sus resultados se conectan a las entradas de un multiplexor 4 a 1 (Select Bits = 2, Data Bits = 4). El selector `Sel[1:0]` controla directamente qué operación llega a la salida `Result`. Para el sumador conecté una constante `0` en su `Cin`, mientras que el restador ya tiene su `Cin = 1` interno.
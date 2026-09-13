# CP1 - Ejercicio 7: Multiplexor y Demultiplexor

## 📋 Enunciado
Implementar en Logisim un multiplexor y un demultiplexor con selectores de 3 bits.

TIP: Implementar multiplexores y demultiplexores con selectores de menor tamaño y utilizarlos en la implementación de multiplexores y demultiplexores con selectores de mayor tamaño.

## 💡 Solución

### Multiplexor 8 a 1
Entradas: `A` a `H` (8 datos de 1 bit), `Sel[2:0]` (3 bits).  
Salida: `Res` (1 bit).

### Demultiplexor 1 a 8
Entradas: `A` (1 dato), `Sel[2:0]` (3 bits).  
Salidas: `R1` a `R8` (8 salidas de 1 bit).

Decidí construir ambos circuitos de forma jerárquica, tal como sugiere el TIP, en lugar de implementar directamente las 8 combinaciones del selector con compuertas. 

Para el MUX, partí de un `MUX 2` (1 selector), lo usé para construir un `MUX 4` (2 selectores), y con dos `MUX 4` más un `MUX 2` construí el `MUX 8` (3 selectores). 

Para el DEMUX seguí el mismo camino: `DEMUX 2` → `DEMUX 4` → `DEMUX 8`, usando la lógica de habilitación con el bit de mayor peso (`Sel3`) para activar el grupo correspondiente. 
# CP1 - Ejercicio 4: Sumador de 4 bits

## 📋 Enunciado
Implementar en Logisim un sumador de dos números de 4 bits.
TIP: Usar el Sumador Completo.

## 💡 Solución
Entradas: `A[3:0]`, `B[3:0]` (4 bits cada una).  
Salidas: `result[4:0]` (5 bits: `Cout` + `Sum[3:0]`).
 
Decidí usar cuatro instancias del subcircuito `Full Adder` conectadas en cascada, tal como sugiere el TIP. El `carry` de salida de cada Full Adder se conecta al `Cin` del siguiente, empezando por `Cin = 0` en el bit menos significativo. Para formar el resultado final de 5 bits, usé un splitter que combina los 4 bits de suma (`Sum[3:0]`) con el carry final (`Cout`) en un solo bus, donde `Cout` ocupa el bit más significativo. Esto permite ver el resultado completo de la suma, incluyendo el desbordamiento, en un solo probe.
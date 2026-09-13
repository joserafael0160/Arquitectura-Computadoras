# CP1 - Ejercicio 8: Decodificador

## 📋 Enunciado
Implementar en Logisim un decodificador con selector de 3 bits.

## 💡 Solución
Entradas: `A`, `B`, `C` (3 bits).  
Salidas: `R0` a `R7` (8 salidas de 1 bit).

Ecuaciones:

`R0 = ¬A ∧ ¬B ∧ ¬C`

`R1 = ¬A ∧ ¬B ∧ C`

`R2 = ¬A ∧ B ∧ ¬C`

`R3 = ¬A ∧ B ∧ C`

`R4 = A ∧ ¬B ∧ ¬C`

`R5 = A ∧ ¬B ∧ C`

`R6 = A ∧ B ∧ ¬C`

`R7 = A ∧ B ∧ C`

Primero pensé en reutilizar la misma lógica jerárquica del ejercicio anterior, construyendo un `Decoder 1a2`, luego un `Decoder 2a4` y finalmente el `Decoder 3a8`. 

Pero me di cuenta de que era innecesario: para 3 bits el decodificador directo son solo 8 compuertas AND, y añadir capas de jerarquía no aportaba ningún beneficio real. 

Decidí implementarlo directamente y, en lugar de dibujar compuertas NOT separadas, activé las burbujas de negación integradas en las entradas de cada AND (`negate0`, `negate1`, `negate2`).
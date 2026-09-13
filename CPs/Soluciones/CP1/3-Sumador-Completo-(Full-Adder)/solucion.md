# CP1 - Ejercicio 3: Sumador Completo (Full Adder)

## 📋 Enunciado
Implementar en Logisim un circuito que realice la suma de dos dígitos binarios, teniendo en cuenta el carry de entrada.

## 💡 Solución
Entradas: `A`, `B`, `Cin` (1 bit).  
Salidas: `Sum`, `Carry` (1 bit).

Ecuaciones:

`Sum = (A ⊕ B) ⊕ Cin`

`Carry = (A ∧ B) ∨ ((A ⊕ B) ∧ Cin)`

 
Decidí usar dos compuertas XOR para la suma: primero calculo `A ⊕ B` y luego lo XOR con `Cin`. Para el carry, reutilizo ese mismo resultado `A ⊕ B` y lo combino con `Cin` mediante una AND, y aparte calculo `A ∧ B` con otra AND. Finalmente, una OR une ambas partes. Esta estructura sigue las ecuaciones, aprovechando el resultado intermedio.
# CP1 - Ejercicio 5: Restador de 4 bits

## 📋 Enunciado
Implementar en Logisim un restador de dos números de 4 bits.
TIP: Usar el Sumador Completo.

## 💡 Solución
Entradas: `A[3:0]`, `B[3:0]` (4 bits cada una).  
Salidas: `Diff[3:0]` (4 bits), `Cout` (1 bit).

Decidí reutilizar el subcircuito `Sumador 4 digitos` del ejercicio anterior en lugar de construir un restador desde cero, aplicando la propiedad del complemento a 2: `A - B = A + ¬B + 1`. 

Para lograrlo, invertí los 4 bits de `B` con una compuerta NOT configurada a 4 bits de ancho, y conecté `Cin = 1` en la entrada del sumador. El resultado de la suma es directamente `Diff`, y el carry final es `Cout`. Añadí probes en las entradas y salidas configurados como decimal sin signo para facilitar la verificación.
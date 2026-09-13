# CP1 - Ejercicio 1: Primeros Pasos con Logisim

## 📋 Enunciado

**a)** Diseñar e implementar la compuerta lógica XOR usando solo compuertas AND, OR y NOT.  
Crear el circuito `MiXOR` con entradas `A`, `B` y salida `C`. Probar con la herramienta "Mano" y crear un circuito `TestMiXOR` que instancie `MiXOR`.

**b)** Crear un circuito que, dados dos números de 4 bits (sin signo), genere su suma en 5 bits.  
Usar un sumador de 4 bits, un splitter para separar el carry, túneles para el acarreo y probes para visualizar en decimal sin signo.

## 💡 Solución

### a) XOR con AND, OR y NOT

La función XOR se puede expresar como:

`C = (A ∧ ¬B) ∨ (¬A ∧ B)`

O equivalentemente:

`C ≡ A ⊕ B`


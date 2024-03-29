# ayudantia-02

martes 21 marzo 2023

# unidad 0: números y ángulos

<!---
## qué deben saber:

- diferencia entre números naturales y reales
- noción de infinito
- qué son los sistemas numéricos
- conversión entre sistemas numéricos distintos
    - sistema decimal
    - sistema binario
    - sistema hexadecimal
- qué es son los ángulos y como se miden
- diferencia entre grados y radianes
- conversión entre grados y radianes
- ¿qué es $\pi$?
--->

## ejercicio-01: números como sumas de potencias

representa los siguientes números decimales como una suma de potencias de 10:

- $2023_{(base10)}$
- $17,456_{(base10)}$
- $1003003_{(base10)}$

<details>
<summary>--- solución ---</summary>

los números que utilizamos día a día está formado por un código de diez símbolos (del 0 al 9). A esto se le llama un código numérico de base 10.

para realizar la suma de potencias de 10 nos debemos fijar en el orden de los números de derecha a izquierda.

el resultado para los números pedidos es:

- $2023_{(base10)} \Rightarrow 2 \cdot 10^3 + 2 \cdot 10^1 + 3 \cdot 10^0$

- $17.456_{(base10)}  \Rightarrow  1 \cdot 10^1 + 7 \cdot 10^0 + 4 \cdot 10^{-1} + 5 \cdot 10^{-2} + 6 \cdot 10^{-2}$

- $1003003_{(base10)} \Rightarrow 1 \cdot 10^6 + 3 \cdot 10^3 + 3 \cdot 10^0$

</details>

## ejercicio-02: números binarios

a) represente los siguientes números binarios como números decimales:

- $11_{(base2)}$
- $1101_{(base2)}$
- $100011_{(base2)}$

<details>
    <summary>--- solución ---</summary>

el sistema binario ocupa solamente dos dígitos (0 y 1).

para convertir cualquier número binario a un número decimal, debemos representar el número como una suma de potencias de 2 y luego sumar.

para el caso del número binario 11, la suma de potencias de dos quedaría:

$$11_{(base2)} \Rightarrow 1 \cdot 2^1 + 1 \cdot 2^0$$

$$= 2 + 1 = 3_{(base10)}$$

$$\therefore \ 11_{(base2)} \Rightarrow 3_{(base10)}$$

para el caso del número binario 1101:

$$1101_{(base2)} \Rightarrow 1 \cdot 2^3 + 1 \cdot 2^2 + 0 \cdot 2^1 + 1 \cdot 2^0$$

$$= 8 + 4 + 0 + 1 \\ = 13_{(base10)}$$

$$\therefore \ 1101_{(base2)} \Rightarrow 13_{(base10)}$$

y para convertir el número binario 100011 a decimal:

$$100011_{(base2)} \Rightarrow 1 \cdot 2^5 + 1 \cdot 2^1 + 1 \cdot 2^0$$

$$= 32 + 2 + 1 \\ = 35_{(base10)}$$

$$\therefore \ 100011_{(base2)} \Rightarrow 35_{(base10)}$$

</details>

b) represente los siguientes números decimales como un números binarios:

- $3_{(base10)}$
- $13_{(base10)}$
- $35_{(base10)}$

<details>
    <summary>--- solución ---</summary>

para convertir un número en base 10 a cualquier otra base, debemos realizar divisiones sucesivas e ir registrando el residuo de esa división.

para convertir $3_{(base10)}$ hacemos lo siguiente:

1. Dividimos $3 \div 2 = 1$ con residuo $1$. este residuo es la primera cifra de nuestro número binario.
2. dividimo $1 \div 2 = 0$ con residuo $1$. este residuo es la segunda cifra de nuestro número binario.

para formar el número binario recopilamos los residuos calculados:

$$\therefore \ 3_{(base10)} \Rightarrow 11_{(base2)}$$

para convertir $13_{(base10)}$ hacemos lo siguiente:

1. Dividimos $13 \div 2 = 6$ con residuo $1$
2. Dividimos $6 \div 2 = 3$ con residuo $0$
3. Dividimos $3 \div 2 = 1$ con residuo $1$
4. Dividimos $1 \div 2 = 0$ con residuo $1$

recopilando los residuos obtenemos:

$$\therefore \ 13_{(base10)} \Rightarrow 1101_{(base2)}$$

Para convertir $35_{(base10)}$ hacemos lo mismo:

1. dividimos $35 \div 2 = 17$ con residuo $1$
2. dividimos $17 \div 2 = 8$ con residuo $1$
3. dividimos $8 \div 2 = 4$ con residuo $0$
4. dividimos $4 \div 2 = 2$ con residuo $0$
5. dividimos $2 \div 2 = 1$ con residuo $0$
6. dividimos $1 \div 2 = 0$ con residuo $1$

recopilando los residuos obtenemos:

$$\therefore \ 35_{(base10)} \Rightarrow 100011_{(base2)}$$

</details>

## ejercicio-03: colores RGB como números hexadecimales

¿qué color representa el código hexadecimal #FC7D26? ¿qué intensidad de rojo, verde y azul posee este color? escriba su respuesta usando números en base 10.

<details>
    <summary>--- solución ---</summary>

usualmente en los sistemas digitales como nuestros computadores o celulares se utilizan números en base hexadecimal para representar los colores del espectro visible, con números que van del 0 a 255.

el código hexadecimal posee 16 símbolos:

| base 10 | 0   | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   | 9   | 10  | 11  | 12  | 13  | 14  | 15  |
| ------- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| base 16 | 0   | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   | 9   | A   | B   | C   | D   | E   | F   |

los códigos de colores poseen 6 cifras hexadecimales. ej: #AA00FF

las dos cifras más a la izquierda representan la intensidad del color rojo, las próximas dos cifras la intensidad del color verde, y las últimas dos cifras la intensidad del color azul.

### analizando el color #FC7D26

el color #FC7D26 tiene FC en rojo, 7D en verde y 26 en azul.

### intensidad de rojo

para convertir la cifra FC a decimal hacemos la multiplicación por potencias de 16:

$$FC_{(base16)} \Rightarrow F \cdot 16^1 + C \cdot 16^0$$

convertimos las letras a números

$$FC_{(base16)} \Rightarrow 15 \cdot 16^1 + 12 \cdot 16^0$$

y calculamos

$$= 240 + 12 = 252$$

$$\therefore \ FC_{(base16)} \Rightarrow 252_{(base10)}$$

por lo tanto este color tiene una intensidad 252 de rojo.

### intensidad de verde

para convertir la cifra 7D a decimal hacemos la multiplicación por potencias de 16:

$$7D_{(base16)} \Rightarrow 7 \cdot 16^1 + D \cdot 16^0$$

convertimos las letras a números decimales

$$7D_{(base16)} \Rightarrow 7 \cdot 16^1 + 13 \cdot 16^0$$

y calculamos

$$= 112 + 13 = 125$$

$$\therefore \ 7D_{(base16)} \Rightarrow 125_{(base10)}$$

por lo tanto este color tiene una intensidad 125 de verde.

### Intensidad de azul

para convertir la cifra 26 a decimal hacemos la multiplicación por potencias de 16:

$$26_{(base16)} \Rightarrow 2 \cdot 16^1 + 6 \cdot 16^0$$

y calculamos

$$= 32 + 6 = 38$$

$$\therefore \ 26_{(base16)} \Rightarrow 38_{(base10)}$$

por lo tanto este color tiene una intensidad 38 de azul.

### conclusión final

finalmente tenemos que este color está formado por la siguiente combinación de colores RGB:

$$\therefore \ FC7D26_{(base16)} \Rightarrow (R,G,B) = (252_{(base10)}, \ 125_{(base10)}, \ 38_{(base10)})$$

este color tiene mucho rojo (cerca del máximo de 255), intensidad moderada de verde y muy poco azul, por lo que se puede concluir que representa un color anaranjado, al ser un sistema aditivo.

</details>

## ejercicio-04: clasificando ángulos

sabiendo que los ángulos se pueden clasificar en los siguientes tipos:

- ángulo agudo (menor a 90 grados)
- ángulo recto (90 grados)
- ángulo obtuso (mayor a 90 grados y menor a 180 grados)
- ángulo llano (180 grados)
- ángulo cóncavo (mayor a 180 grados)
- ángulo completo (360 grados)

clasifica los siguientes ángulos que fueron medidos en radianes:

1. ángulo de $\frac{\pi}{2} \ rad$
2. ángulo de $\pi \ rad$
3. ángulo de $\frac{3}{2} \pi \ rad$
4. ángulo de $\frac{\pi}{4} \ rad$
5. ángulo de $\frac{\pi}{8} \ rad$
6. ángulo de $2 \pi \ rad$

<details>
<summary>--- solución ---</summary>

para resolver lo pedido es necesario saber que $360°$ equivalen a $2 \pi \ rad$.

1. es un ángulo recto ya que $\frac{\pi}{2} \ rad$ corresponden a $90°$
2. es un ángulo llano ya que $\pi \ rad$ equivalen a $180°$
3. es un ángulo cóncavo ya que $\frac{3}{2} \pi \ rad$ corresponden a $270°$ (tres veces $90°$).
4. es un ángulo agudo ya que $\frac{\pi}{4} \ rad$ corresponden a $45°$
5. es un ángulo agudo ya que $\frac{\pi}{8} \ rad$ corresponden a $22.5°$
6. es un ángulo completo ya que $2 \pi \ rad$ corresponden a $360°$
</details>

## ejercicio-05: de grados a radianes y viceversa

utilizando la ecuación:

$$\frac{2 \cdot \pi \cdot radianes}{360 \cdot grados} = \frac{X \cdot radianes}{Y \cdot grados}$$

a) transforme los siguientes ángulos de grados a radianes:

- $47°$
- $23°$
- $195°$

<details>
<summary>--- solución ---</summary>

- para transformar $47°$ a radianes reemplazamos en la ecuación y calculamos:

$$\frac{2 \pi}{360°} = \frac{X}{47°}$$

$$X = \frac{2 \pi \cdot 47°}{360°}$$

$$X = 0.261 \pi \ rad$$

- para transformar $23°$ a radianes reemplazamos en la ecuación y calculamos:

$$\frac{2 \pi}{360°} = \frac{X}{23°}$$

$$X = \frac{2 \pi \cdot 23°}{360°}$$

$$X = 0.128 \pi \ rad$$

- para transformar $195°$ a radianes reemplazamos en la ecuación y calculamos:

$$\frac{2 \pi}{360°} = \frac{X}{195°}$$

$$X = \frac{2 \pi \cdot 195°}{360°}$$

$$X = 1.083 \pi \ rad$$

</details>

b) transforme los siguientes ángulos de radianes a grados:

- $0.6 \pi \ rad$
- $1.2 \pi \ rad$
- $0.23 \pi \ rad$

<details>
<summary>--- solución ---</summary>

- para transformar $0.6 \ rad$ a grados reemplazamos en la ecuación y calculamos:

$$\frac{2 \pi}{360°} = \frac{0.6 \pi \ rad}{Y}$$

$$Y = \frac{0.6 \pi \cdot 360}{2\pi}$$

$$Y = 108°$$

- para transformar $1.2 \pi \ rad$ a grados reemplazamos en la ecuación y calculamos:

$$\frac{2 \pi}{360°} = \frac{1.2 \pi \ rad}{Y}$$

$$Y = \frac{1.2 \pi \cdot 360}{2\pi}$$

$$Y = 216°$$

- para transformar $0.23 \pi \ rad$ a grados reemplazamos en la ecuación y calculamos:

$$\frac{2 \pi}{360°} = \frac{0.23 \pi \ rad}{Y}$$

$$Y = \frac{0.23 \pi \cdot 360}{2\pi}$$

$$Y = 41.4°$$

</details>

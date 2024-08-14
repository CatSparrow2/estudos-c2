#### Funções Contínuas

* Exponencial
		`f(x) = x³`
* Trigonométrica
		`f(x) = sen(x)`
* Polinomial
		`f(x) = 2x + 5y + z³`
* Logarítmica
		`f(x) = ln(x)`
* Racional
		`f(x)=x2−42x2+3x−5​`
  
$$
f(x) = \frac{P(x)}{Q(x)} 
$$
___
#### Derivadas Normais (C1)

$$
K' = 0
$$
___

$$
x' = 1
$$
___

$$
k.x = k
$$
___

$$
x^3 = 3.x^2
$$
___

$$
√x = \frac{1}{(2√x)} 
$$
___

$$
e^x = e^x 
$$
___

$$
lnx = \frac{1}{x}
$$
___

$$
Sin(x) = Cos(x)
$$
___

$$
cos(x) = - Sin(x)
$$
___

#### Derivadas Parciais


$$
\frac{δz}{δx}(3yx²) = 3y2x = 6xy
$$
___
$$
\frac{δz}{δx}(cos(X, Y)) = -sen(X, Y) * \frac{δ}{δx}(X)
$$
___
$$
\frac{δz}{δx}(sen(X, Y)) = cos(X, Y) * \frac{δ}{δx}(X)
$$
___
##### Exemplos
___
##### Derivada Parcial com Regra da Cadeia e expressões Trigonométrica
![image](https://github.com/user-attachments/assets/78517fbc-2fe6-4ef6-8d98-4b99b4392b69)

___
##### Derivada Parcial com Raiz e Regra da Cadeia
![image](https://github.com/user-attachments/assets/90c9057a-aa36-44f0-8e68-0347c60c297f)

___

##### Regra da Cadeia
![image](https://github.com/user-attachments/assets/217f9cec-7495-4316-9adb-b2e8e5aa1015)

#### Vetor Gradiente
___
**Calcula as derivadas parciais da função em relação à *x* e a *y*, e aplica os pontos nos resultados
___

$$
∇f(p)=<\frac{δf}{δx}(x)(p), \frac{δf}{δy}(y)(p)>
$$
___
ex.: 
	f(x,y) = x² + y²
	p = (1, 1)
```
δz/δx = 2x + 0 = 2x
δz/δy = 2y + 0 = 2y
∇f (1, 1) = <2x, 2y>
∇f (1, 1) = <2.1, 2.1>
∇f (1, 1) = <2, 2>
```

#### Valores extremos de uma função
	Devemos encontrar os "Pontos Críticos", os "Máximos" e os "Mínimos" da função. Existe vários jeitos de fazer isso.

##### Modo 1

1. **Deriva a função em relação a cada variável
2. **Iguala a ZERO
3. **Encontrar os PONTOS CRÍTICOS (valores que zeram as funções)
4. **Calcular o DETERMINANTE DA MATRIZ das DERIVADAS PARCIAIS SECUNDÁRIAS

$$
D =
\left(\begin{array}{cc} 
Fxx & Fyy\\
Fyx & xy
\end{array}\right)
= Fxx.Fyy + Fxy²
$$

5. Substitui os "X"s e "Y"s pelos **PONTOS CRÍTICOS**
   ex.: se os pontos críticos forem 0, 1 e -1

$$
\left(\begin{array}{cc} 
(0,0) & (0,1) & (0,-1)\\
(1,0) & (1,1) & (1,-1)\\
(-1,0) & (-1,1) & (-1,-1)
\end{array}\right)
$$

7. Verifica se:

![image](https://github.com/user-attachments/assets/7ae48f2c-aa69-4927-bedc-f3021f16ede5)


##### Exemplo

![image](https://github.com/user-attachments/assets/20bd8ca2-9cf7-4aa5-b1ea-5b75cbb5cba5)


___
#### Multiplicadores de Lagrange
	Calcula-se o gradiente da função f(x,y) mediante a uma condicional g(x,y)
	
$$
	∇f(x,y) = λ.∇g(x,y)
$$
* Terá duas funções, a **OBJETIVA** e a **CONDICIONAL**. A condicional pode ser que tenha que descobrir 👍.
* Calcula o gradiente da *objetiva (f)* e da *condicional (g)*
* Aplica na fórmula acima, multiplicando o gradiente da *condicional* com a λ
* Iguala as gradientes formando um sistema
* Resolve o sistema descobrindo os valores de *X* e *Y*
* Aplica os valores substituindo na função *condicional*
* O resultado aplica na função *objetiva*

![image](https://github.com/user-attachments/assets/3a0d9b9a-be2c-4c02-a8e9-403847fa7e2e)

___
#### Derivada Direcional

$$
\frac{δf}{δu}(p)=∇f(p).u
$$
1. Calcula o **GRADIENTE** da função
2. Substitui as variáveis pelos valores do **PONTO**
3. Multiplica o resultado pelo **VETOR UNITÁRIO**
   obs.: se for dad um valor no formato "xi ± yj ±...", deve transformar no vetor unitário:

$$
	|u|=√(i²+j²)
$$

$$
	u=\frac{<i,j>}{|u|}
$$

![image](https://github.com/user-attachments/assets/38fa2294-d63d-48ea-880f-ac27f06a4ff3)

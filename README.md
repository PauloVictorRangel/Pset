### Pset

**Respostas do Pset**

**1º Questão**

-	altura: 1
-	largura: 4
-	pixels: [29, 89, 136, 200]

Fórmula para o calculo da inversa:
-# c = 255 - o

- (c = inversa e o = original)

Respostas:
-c = 255 - 39 = 226
-c = 255 - 89 = 166
-c = 255 - 136 = 119
-c = 255 - 200 = 55

• Para calcular a inversa usaremos o valor 255(valor_maximo(branco)), e subtrai o valor que será utilizado, então conseguirá a cor desejada.

**2º Questão**

• usaremos (test_images/bluegill.png) como a imagem, ao passar a imagem pelo filtro de inversão e salvar, nos retorna a imagem inversa.

**Resultado**

![peixeIn](https://github.com/PauloVictorRangel/Pset/assets/104431068/5939b4ea-10a6-4b66-a8a3-b53a2e961141)

**3º Questão**

 - Com o Kernel definido, começaremos da esquerda para a direita de cima para baixo, e contaremos pelas linhas de x, y
 - Temos o pixel central que é x,y.
 
 - Usando a formula:
 -#Ox,y = Ix,y * Kx,y
 
- Ox,y = Ix,y -1 * K0,1 = 53 * -0,07 = -3,71 
- Ox,y = Ix,y -1 * K1,0 = 129 * -0,45 = -58,05
- Ox,y = Ix,y -1 * K1,2 = 148 * -0,25 = -37
- Ox,y = Ix,y -1 * K2,1 = 174 * -0,12 = -20,88 
- Ox,y = Ix,y -1 * K1,1 = 127 * 1,20 = 152,4 

- [ 0  -3,71  0]
- [58,05  152,4  -37]
- [0   -20,88  0]

Calculando:
- (-3,71 + (-58,05) + (-37) + (-20,88) + 152,4) = 32,7 ~= 33

**4º Questão**
![Porco_Passaro_correlacionado](https://github.com/PauloVictorRangel/Pset/assets/104431068/431a02cf-b0e3-42e0-a5d7-d54229658849)
Imagem correlacionada
 
 **5º Questão**
 
Vamos utilizar um kernel chamado “caixa de desfoque ou box blur”,
o resultado dos pixels de uma imagem será a média dos pixels vizinhos da imagem original(entrada).


**6º Questão**

O kernel kx e ky aplicam um filtro para borrar as bordas, só que kx aplica esse filtro nas bordas horizontais da imagem e o ky aplica esse filtro nas bordas verticais da imagem.

- Ox,y = round(√Ox^2x,y + Ou^2x,y)



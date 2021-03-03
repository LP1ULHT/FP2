**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

*Linguagens de Programação I - 2019/2020*

# Ficha de Exercícios - 2

Na resolução destes exercícios deve ser utilizada a Linguagem de Programação C. Para além da correta implementação dos requisitos, tenha em conta os seguintes aspetos:

- O código apresentado deve ser bem indentado. 
- O código deve compilar sem erros ou *warnings* utilizando o *gcc* com as seguintes flags:
- `gcc -ansi -Wall -Wextra -Wpedantic -ansi -g exercicio1.c -o exercicio1`
- Tenha em atenção os nomes dados das variáveis, para que sejam indicadores daquilo que as mesmas vão conter.
- Evite o uso de constantes mágicas. 
- Evite duplicação de código. 
- Considere a implementação de funções para melhorar a legibilidade, evitar a duplicação e criar soluções mais genéricas.


1. O que faz o seguinte programa?

   ```c
   #include <stdio.h>
   
   int main(void)
   {
   	int x;
   	scanf( "%d", &x );
   	printf("%d\n", 2*x );
   	return 0;
   }
   ```

2. Leia uma temperatura em graus Fahrenheit e apresente-a convertida em graus Celsius. A fórmula de conversão é: C = 5.0 ∗ (F − 32.0)/9.0, sendo C é a temperatura em graus Celsius e F a temperatura em graus Fahrenheit. 

3. Leia o valor do raio de um círculo. Calcule e imprima a área do círculo correspondente. A área do círculo é π ∗ raio² , considere π = 3.141592 (constante).

4. Faça um programa que peça ao utilizador 2 valores inteiros e coloque o primeiro valor numa variável chamada de A e o segundo valor noutra variável chamada de B. Em seguida, o seu programa deverá trocar o conteúdo destas variáveis e imprimir no ecrã o que cada variável contém.
   
5. Faça um programa que peça ao utilizador 4 valores inteiros. Coloque estes valores nas variáveis a, b, c, d e imprima no ecrã o resultado da seguinte expressão:(a + b + c) x d
   
6. Faça um programa que peça ao utilizador 4 notas de um aluno e imprima no ecrã a média desse aluno. 
   
7. Considere um programa com as seguintes variáveis e respetivas inicializações:

    `unsigned char c = 3.14;` 
    `unsigned short int i = 3.14; `
    `unsigned int j = 'B'; `
    `float f = 'C'; `

    Usando o debugger (sem recorrer a `printf()`) verifique:

    - Qual é o valor efetivo `f`?

    - Qual o valor das variáveis quando se soma o valor 2 a cada uma delas?

8. Faça um programa que, a partir da leitura  das medidas dos lados de um retângulo (comprimento e largura), lidos do teclado, calcule e imprima a área e o perímetro do retângulo.

9. Faça um programa que leia pelo teclado um valor, em euros, converta e imprima o mesmo num valor     em dólares. Considere que €1 seja equivalente a US$ 1,23.

10. A condição física de uma pessoa pode ser medida com base no cálculo do Índice de Massa Corporal     (IMC). O mesmo é calculado dividindo-se o peso desta pessoa em kg pelo quadrado da sua altura em m. Escreva um programa que leia o peso em kilograma e a altura de uma pessoa em metros, calcule e mostre o IMC. 

    *Se as entradas fossem 70.0kg para o peso e 1.80m para altura então a saída esperada seria aproximadamente 21.60.*

11. Escreva um programa que lê um certo número de segundos e dá o correspondente aos Dias, Horas, Minutos e Segundos.

     *Exemplo: 228184 segundos correspondem a 2 Dias e 15 Horas 23 Minutos e 4 Segundos.*

12. A importância de €780.000,00 será dividida entre três vencedores de um concurso. Sendo que da quantia total:

    - O primeiro vencedor receberá 46%

    - O segundo receberá 32%

    - O terceiro receberá o restante

    Calcule e imprima a quantia ganha por cada um dos vencedores.


13. Faça um programa que leia um número inteiro e o imprima.

   

14. Faça um programa que leia um número real e o imprima.

   

15. Peça ao utilizador para digitar três valores inteiros e imprima a soma deles.

   

16. Leia um número real e imprima o resultado do quadrado desse número.

   

17. Crie um programa capaz de ler um caractere e imprimir o seu valor em decimal e hexadecimal.

   

18. Preencha a seguinte tabela com o resultado esperado (0 ou 1) depois de aplicar o “operador lógico” aos dois valores indicados.

| Valor 1 | Operador | Valor 2 | Resultado |
| ------- | -------- | ------- | --------- |
| 1       | &&       | 0       |           |
| 10      | &&       | 1       |           |
| 0       | &&       | 0       |           |
| 1       | \|\|     | 10      |           |
| 10      | \|\|     | 0       |           |
| 0       | \|\|     | 0       |           |



19. Indique qual o resultado das seguintes expressões. Assuma que todas as variáveis são inteiras:

- X = 5 && 6; 
- X = 5 && 0; 
- X = 5 > 2; 
- X = 5==6; 
- X = !5; 
- X = !0; 
- X = 5­3­2 || 1; 
- X = 5­6 || 1; 
- X = 5­7 || 0; 
- X = 0*3 || 5*0; 
- X = 0 || !0; 
- X = 50 >> 2; 
- X = 100 << 3

   

20. Implemente uma função que recebe o número de quilómetros que percorreu e o número de litros de combustível que o automóvel consumiu e retorne o número de litros que este consome em média em 100 quilómetros. Use constantes para representar os vários fatores de conversão.

   *Exemplo de uma sessão de uso do programa (à frente do símbolo ‘>’ aparece o input do utilizador):*

   ```bash
   Qual o número de quilómetros que percorreu?
   > 100
   Qual o número de litros que consumiu?
   > 10
   Consumo aos 100 Km = 10
   ```
   
   
   

21. Implemente uma função que recebe um horário, através da Hora, dos Minutos e dos Segundos, e com estes dados calcule e retorne o tempo total em segundos.

   *Exemplo de uma sessão de uso do programa:*

   ```bash
   Qual a hora?
   > 10
   Qual o minuto?
   > 20
   Qual o segundo?
   > 35
   Total de segundos = 37235
   ```

   

22. Implemente um programa que peça ao utilizador para introduzir dois números inteiros (a e b) e, de seguida, apresente no ecrã o resultado das seguintes operações aritméticas:

   - a+b

   - a-b (assim com b-a)

   - a*b

   - a/b (assim como b/a)
   
     

   *Notas:* 

- Deve ter em conta que o operador de divisão, quando aplicado a dois números inteiros, descarta a parte fracionária do resultado. Neste exercício, se o utilizador introduzir o valor 1 para o primeiro número e o valor 2 para o segundo número, o programa deve apresentar o valor 0.5 como resultado de a / b.

- 
  Deve ter em atenção situações de erro possíveis. Por exemplo, quando o utilizador introduzir 50 para o primeiro número e o valor 0 para o segundo número, não deve ser executada a operação a/b .

- Deve ter em atenção situações de erro possíveis. Por exemplo, quando o utilizador introduzir o valor 50 para o primeiro número e o valor 0 para o segundo número, não deve ser executada a operação a/b (pois seria 50/0.

  

23. Considere o seguinte programa em C:

    ```C
    # include <stdio.h>
    int main (void)
    {
    	char alpha = (char) 0xF0;
    	unsigned int clr = 0xBF3F3FF0 ;
    	unsigned char beta;
    	unsigned char gr = (clr >> 16) & (0x000000FF);
    	beta = alpha >> 4;
    	return 0;
    }
    ```

    - Calcule, manualmente e sem compilar o código, o valor das variáveis `alpha`, `beta`, `clr` e `gr`.
    - A variável beta é um número negativo ou positivo?
    - Compile o código e verifique se o resultado foi o esperado. Caso não seja, identifique o erro e volte a fazer a primeira alínea.



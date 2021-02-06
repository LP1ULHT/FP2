**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

*Linguagens de Programação I - 2019/2020*

# Ficha de Exercícios - 2

Na resolução destes exercícios deve ser utilizada a Linguagem de Programação C. Para além da correta implementação dos requisitos, tenha em conta os seguintes aspetos:

- O código apresentado deve ser bem indentado. 
- O código deve compilar sem erros ou *warnings* utilizando o *gcc* com as seguintes flags:
- `gcc -Wall -Wextra -Wpedantic -std=c99 -g exercicio1.c -o exercicio1`
- Tenha em atenção os nomes dados das variáveis, para que sejam indicadores daquilo que as mesmas vão conter.
- Evite o uso de constantes mágicas. 
- Evite duplicação de código. 
- Considere a implementação de funções para melhorar a legibilidade, evitar a duplicação e criar soluções mais genéricas.



1. Faça um programa que leia um número inteiro e o imprima.

   

2. Faça um programa que leia um número real e o imprima.

   

3. Peça ao utilizador para digitar três valores inteiros e imprima a soma deles.

   

4. Leia um número real e imprima o resultado do quadrado desse número.

   

5. Crie um programa capaz de ler um caractere e imprimir o seu valor em decimal e hexadecimal.

   

6. Preencha a seguinte tabela com o resultado esperado (0 ou 1) depois de aplicar o “operador lógico” aos dois valores indicados.

| Valor 1 | Operador | Valor 2 | Resultado |
| ------- | -------- | ------- | --------- |
| 1       | &&       | 0       |           |
| 10      | &&       | 1       |           |
| 0       | &&       | 0       |           |
| 1       | \|\|     | 10      |           |
| 10      | \|\|     | 0       |           |
| 0       | \|\|     | 0       |           |



7. Indique qual o resultado das seguintes expressões. Assuma que todas as variáveis são inteiras:

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

   

8. Implemente uma função que recebe o número de quilómetros que percorreu e o número de litros de combustível que o automóvel consumiu e retorne o número de litros que este consome em média em 100 quilómetros. Use constantes para representar os vários fatores de conversão.

   *Exemplo de uma sessão de uso do programa (à frente do símbolo ‘>’ aparece o input do utilizador):*

   ```bash
   Qual o número de quilómetros que percorreu?
   > 100
   Qual o número de litros que consumiu?
   > 10
   Consumo aos 100 Km = 10
   ```
   
   
   

9. Implemente uma função que recebe um horário, através da Hora, dos Minutos e dos Segundos, e com estes dados calcule e retorne o tempo total em segundos.

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

   

10. Implemente um programa que peça ao utilizador para introduzir dois números inteiros (a e b) e, de seguida, apresente no ecrã o resultado das seguintes operações aritméticas:

   - a+b

   - a-b (assim com b-a)

   - a*b

   - a/b (assim como b/a)
   
     

   *Notas:* 

- Deve ter em conta que o operador de divisão, quando aplicado a dois números inteiros, descarta a parte fracionária do resultado. Neste exercício, se o utilizador introduzir o valor 1 para o primeiro número e o valor 2 para o segundo número, o programa deve apresentar o valor 0.5 como resultado de a / b.

- 
  Deve ter em atenção situações de erro possíveis. Por exemplo, quando o utilizador introduzir 50 para o primeiro número e o valor 0 para o segundo número, não deve ser executada a operação a/b .

- Deve ter em atenção situações de erro possíveis. Por exemplo, quando o utilizador introduzir o valor 50 para o primeiro número e o valor 0 para o segundo número, não deve ser executada a operação a/b (pois seria 50/0.

  

11. Considere o seguinte programa em C:

    ```C
    # include <stdio.h>
    int main (void)
    {
    	char alpha = (char) 0xF0;
    	unsigned int clr = 0xBF3F3FF0 ;
    	unsigned char beta;
    	unsigned char gr = (clr >> 16) & (0 x000000FF);
    	beta = alpha >> 4;
    	return 0;
    }
    ```

    - Calcule, manualmente e sem compilar o código, o valor das variáveis `alpha`, `beta`, `clr` e `gr`.
    - A variável beta é um número negativo ou positivo?
    - Compile o código e verifique se o resultado foi o esperado. Caso não seja, identifique o erro e volte a fazer a primeira alínea.



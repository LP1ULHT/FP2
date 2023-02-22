**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

*Linguagens de Programação I*

# Ficha de Exercícios - 2

>Na resolução destes exercícios deve ser utilizada a Linguagem de Programação C. Para além da correta implementação dos requisitos, tenha em conta os seguintes aspetos:
>* O código apresentado deve ser bem indentado. 
>* O código deve compilar sem erros ou *warnings* utilizando o *gcc* com as seguintes flags: `-Wvla -Wall -Wextra -Wpedantic -g -Wdeclaration-after-statement`
>* Tenha em atenção os nomes dados das variáveis, para que sejam indicadores daquilo que as mesmas vão conter.
>* Evite o uso de constantes mágicas. 
>* Evite duplicação de código. 
>* Considere a implementação de funções para melhorar a legibilidade, evitar a duplicação e criar soluções mais genéricas.


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

3. Faça um programa que peça ao utilizador 2 valores inteiros e coloque o primeiro valor numa variável chamada de A e o segundo valor noutra variável chamada de B. Em seguida, o seu programa deverá trocar o conteúdo destas variáveis e imprimir no ecrã o que cada variável contém.
   

4. Escreva um programa que declara um número real de dupla precisão e o inicializa com a seguinte expressão:
```C
double a = (0.3 * 3) - 0.9;
```
O programa em seguida testa se o número é zero. Execute o programa compilado. O que observa? 


5. Faça um programa que peça ao utilizador 4 notas de um aluno e imprima no ecrã a média desse aluno. 
   
   5.1 Altere o programa de forma a que, para além da média, o programa apresente as 4 notas por ordem crescente.


6. Considere um programa com as seguintes variáveis e respetivas inicializações:

    `unsigned char c = 3.14;` 
    `unsigned short int i = 3.14; `
    `unsigned int j = 'B'; `
    `float f = 'C'; `

    Usando o debugger (sem recorrer a `printf()`) verifique:

    - Qual é o valor efetivo `f`?

    - Qual o valor das variáveis quando se soma o valor 2 a cada uma delas?


7. Escreva um programa que lê um certo número de segundos e dá o correspondente aos Dias, Horas, Minutos e Segundos.

     *Exemplo: 228184 segundos correspondem a 2 Dias e 15 Horas 23 Minutos e 4 Segundos.*

   


8. Preencha a seguinte tabela com o resultado esperado (0 ou 1) depois de aplicar o “operador lógico” aos dois valores indicados.

| Valor 1 | Operador | Valor 2 | Resultado |
| ------- | -------- | ------- | --------- |
| 1       | &&       | 0       |           |
| 10      | &&       | 1       |           |
| 0       | &&       | 0       |           |
| 1       | \|\|     | 10      |           |
| 10      | \|\|     | 0       |           |
| 0       | \|\|     | 0       |           |



9. Indique qual o resultado das seguintes expressões. Assuma que todas as variáveis são inteiras:

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

   

10. Implemente uma função que recebe o número de quilómetros que percorreu e o número de litros de combustível que o automóvel consumiu e retorne o número de litros que este consome em média em 100 quilómetros. Use constantes para representar os vários fatores de conversão.

   *Exemplo de uma sessão de uso do programa (à frente do símbolo ‘>’ aparece o input do utilizador):*

   ```bash
   Qual o número de quilómetros que percorreu?
   > 200
   Qual o número de litros que consumiu?
   > 20
   Consumo aos 100 Km = 10
   ```
   
   
   

11. Implemente uma função que recebe um horário, através da Hora, dos Minutos e dos Segundos, e com estes dados calcule e retorne o tempo total em segundos.

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

   

12. Implemente um programa que peça ao utilizador para introduzir dois números inteiros (a e b) e, de seguida, apresente no ecrã o resultado das seguintes operações aritméticas:

   - a+b

   - a-b (assim com b-a)

   - a*b

   - a/b (assim como b/a)
   
     

   *Notas:* 

- Deve ter em conta que o operador de divisão, quando aplicado a dois números inteiros, descarta a parte fracionária do resultado. Neste exercício, se o utilizador introduzir o valor 1 para o primeiro número e o valor 2 para o segundo número, o programa deve apresentar o valor 0.5 como resultado de a / b.

- 
  Deve ter em atenção situações de erro possíveis. Por exemplo, quando o utilizador introduzir 50 para o primeiro número e o valor 0 para o segundo número, não deve ser executada a operação a/b .

- Deve ter em atenção situações de erro possíveis. Por exemplo, quando o utilizador introduzir o valor 50 para o primeiro número e o valor 0 para o segundo número, não deve ser executada a operação a/b (pois seria 50/0.

  

13. Crie um programa capaz de ler um número inteiro em base decimal, octal ou hexadecimal e o converta para as três bases.
   ```bash
   Qual a base do numero que quer inserir? ('d' - decimal, 'o' - octal, 'h' - hexadecimal)
   > h
   Insira o número:
   > A
   Conversao para Decimal: 10
   Conversao para Octal: 12
   Conversao para Hexadecimal: A
   ```




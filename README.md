# Códigos em C - Feitos por mim (para estudo)

 ## - Printf e Scanf (Somente)
<img src="https://img.shields.io/badge/FEITO NO-%2BEMBARCADEIRO-red">

 ### 1-) Nome e idade.
 
 ```c
#include <stdio.h>
	
int main() {
     char nome[50];
     int idade;
	
     printf("Digite seu nome: ");
     scanf("%49s", nome);
    
     printf("Digite sua idade: ");
     scanf("%d", &idade);

     printf("Seu nome eh %s, e sua idade eh %d", nome, idade);
	  
     return 0;
}
```

### 2-) Soma, subtração e multiplicação de números inteiros.

```c
#include <stdio.h>
	
int main() {
    int n1, n2, soma, multiplicacao, subtracao;

    printf("Digite o primeiro numero: ");
    scanf("%d", &n1);

    printf("Digite o segundo numero: ");
    scanf("%d", &n2);
	 
    soma = n1 + n2;
    subtracao = n1 - n2;
    multiplicacao = n1 * n2;
   	 
    printf("A soma dos 2 numeros: %d\n", soma);
    printf("A subtracao dos 2 numeros: %d\n", subtracao);
    printf("A multiplicacao dos 2 numeros: %d\n", multiplicacao);
	   
    return 0;
}
```
### 3-) Média de 2 notas.

```c
#include <stdio.h>
	
int main() {
   	char nome[50];
   	float n1, n2, media = 0;
	
   	printf("Digite o nome do aluno: ");
   	scanf("%49s", nome);
   	 printf("Digite a primeira nota: ");
   	 scanf("%d", &n1);
   	  printf("Digite a segunda nota: ");
	     scanf("%d", &n2);
	   
	   media = (n1 + n2) / 2.0;
	
   	printf("O nome do aluno eh %s, e sua nota eh %.2f", nome, media);
	
   	return 0;
}
```
### 4-) Conversão de temperatura de °C para °F.

```c
#include <stdio.h>
	
int main() {
   	float celcius = 0, fahrenheit = 0;
	
   	printf("Digite a temperatura em Celcius:   ");
   	scanf("%f", &celcius);
    
     fahrenheit = (celcius * 9.0/5.0) + 32;
	
    printf("A temperatura convetida em     Fahrenheit eh: %.2f", fahrenheit);
		   
	   return 0;
}
```
### 5-) Dados pessoais.

```c
#include <stdio.h>
	
int main() {
    char sexo[20];
    float altura = 0;
    int idade = 0;
    
    printf("Digite seu sexo (Feminino ou Masculino): ");
    scanf("%19s", sexo);
     printf("Digite sua altura (sem virgulas): ");
     scanf("%f", &altura);
      printf("Digite sua idade: ");
      scanf("%d", &idade);
      
    printf("Seu sexo eh %s, sua altura eh %.2f, e sua idade eh %d", sexo, altura, idade);
		   
	   return 0;
}
```
## - If, Else If, Else
 <img src="https://img.shields.io/badge/FEITO NO-EMBARCADEIRO-brightgreen">

### 1-) Número positivo, negativo ou zero.

```c
#include <stdio.h>
	
int main() {
    int num;
    
    printf("Digite o numero: ");
    scanf("%d", &num);
    
     if (num > 1) 
	    {
        	printf("Positivo");
     }
     else if (num < -1)
	    {
        	printf("Negativo"); 	
     }
     else 
	    {
        	printf("Eh zero (0)");
	    }
	 	   
	   return 0;
}
```
### 2-) Aprovação escolar.

```c
#include <stdio.h>

int main() {
    int media = 0;

    printf("Digite a média do aluno: ");
    scanf(%d", &media);

    if (media >= 7)
    {   
        printf("Aprovado");
    }
    else if (media >= 5)
    {
      	 printf("Recuperação");
    }
    else
    {
      	 printf("Reprovado");
    }

    return 0;
}
```
....

do While 10 exercícios.. depois editar

```c
#include <stdio.h>

int main() {

    float n1, n2;
    int opcao;

    do
    {  
        printf("\n---Menu de Opções da Calculadora---\n");
        
        printf("\n1- Soma\n");
        printf("2- Subtração\n");
        printf("3- Multiplicação\n");
        printf("4- Divisão\n");
        printf("5- Sair do menu\n");
        
        printf("\nDigite um número das opções acima: ");
        scanf("%d", &opcao);
        
         if (opcao >= 1 && opcao <= 4)
         {
            printf("\nDigite o primeiro número: ");
            scanf("%f", &n1);
             printf("Digite o segundo número: ");
             scanf("%f", &n2);
         }    
        
         switch (opcao)
         {    
             case 1:
                  printf("\nO Resultado da Soma eh: %.2f\n", n1 + n2);
                  break;
             
             case 2:
                  printf("\nO Resultado da Subtração eh: %.2f\n", n1 - n2);   
                  break;
             
             case 3:
                  printf("\nO Resultado da Multiplicação eh: %.2f\n", n1 * n2);
                  break;
                  
             case 4:
                  if (n2 != 0)
                  {  
                     printf("\nO Resultado da Divisão eh: %.2f\n", n1 / n2);
                  }
                  else    
                  {
                     printf("\nNão eh possível dividir por 0\n");
                  }
                  break;
                  
             case 5:
                  printf("\nSaindo do Menu da Calculadora\n");
                  break;
             
             default:
                  printf("\nOpção Inválida\n");
                  break;
         }       
           
    } while (opcao != 5);

    return 0;
}
```
......

```c
#include <stdio.h>
#include <string.h>

int main() {

    char sC[7] = "Github", sD[10];
    int contador = 0, parar = 0;

    do
    {  
        printf("\nDigite a sua senha (você tem 3 tentativas): ");
        scanf("%9s", sD);
        contador++;
        
         if (strcmp(sD, sC) == 0)
         {
             printf("\nSenha Correta\n");
             parar = 1;
         }
         else
         {
             printf("\nSenha Incorreta, tente novamente!\n");
         }    
         
    }while (contador < 3 && parar == 0);
    
    if (parar == 0)
    {
        printf("\nSuas tentivas acabaram");
    }
    
    return 0;
}
```

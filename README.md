# Códigos em C - Feitos por mim

 Printf e Scanf

 1-) Nome e idade.

#include <stdio.h>
int main (){
	
	char nome[50];
	int idade;
	
	printf("Digite seu nome: ");
	scanf("%s", &nome);
	 printf("Digite sua idade: ");
	 scanf("%d", &idade);
	 
	  printf("Seu nome eh %s, e sua idade eh %d", nome, idade);
	  
	  return 0;	
}

2-) Soma, subtração e multiplicação de números inteiros.

#include <stdio.h>
int main (){
	
	int n1, n2, soma, multiplicacao, subtracao;
	
	soma = 0;
	multiplicacao = 0;
	subtracao = 0;
	
	printf("Digite o primeiro numero: ");
	scanf("%d", &n1);
	 printf("Digite o segundo numero: ");
	 scanf("%d", &n2);
	 
	 soma = n1 + n2;
	 subtracao = n1 - n2;
	 multiplicacao = n1 * n2;
	 
	   printf("A soma dos 2 numeros: %d\n", soma);
	   printf("A subtracao dos 2 numeros %d\n", subtracao);
	   printf("A multiplicacao dos 2 numeros: %d\n", multiplicacao);
	   
	   return 0;
}

3-) Média de 2 notas.

#include <stdio.h>
int main (){
	
	char nome[50];
	int n1, n2;
	float media;
	
	media = 0;
	
	printf("Digite o nome do aluno: ");
	scanf("%s", &nome);
	printf("Digite a primeira nota: ");
	scanf("%d", &n1);
	printf("Digite a segunda nota: ");
	scanf("%d", &n2);
	
	media = (n1 + n2) / 2.0;
	
	printf("O nome do aluno eh %s, e sua nota eh %.1f", nome, media);
		   
	return 0;
}

4-) Conversão de temeperatura de °C para °F.

#include <stdio.h>
int main (){
	
	float celcius, fahrenheit;
	
	fahrenheit = 0;
	celcius = 0;
	
	printf("Digite a temperatura em Celcius: ");
	scanf("%f", &celcius);
    
     fahrenheit = (celcius * 9.0/5.0) + 32;
	
	  printf("A temperatura convetida em Fahrenheit eh: %.1f", fahrenheit);
		   
	return 0;
}

5-) Dados pessoais.

#include <stdio.h>
int main (){
	
    char sexo[50];
    float altura;
    int idade;
    
    altura = 0;
    idade = 0;
    
    printf("Digite seu sexo (Feminino ou Masculino): ");
    scanf("%s", &sexo);
     printf("Digite sua altura (sem virgulas): ");
     scanf("%f", &altura);
      printf("Digite sua idade: ");
      scanf("%d", &idade);
      
      printf("Seu sexo eh %s, sua altura eh %.2f, e sua idade eh %d", sexo, altura, idade);
		   
	return 0;
}




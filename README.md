# questao12

Ponteiros para função serve principalmente para definir, em tempo de execução, qual função será executada, sem a necessidade de escrever
o nome da função de forma explícita naquele ponto do código.
exemplo de código
 #include <stdio.h>
 #include <stdlib.h>
 
 int soma(int a, int b){
  return a + b;
  }
 
 itn main(){
    int x, y, z;
    int (*p)(int, int); //ponteiro para int que recebe 2 parametros
    printf("Digite dois numeros: ");
    scanf("%d %d", &x,&y);
    p = soma  //associaçao do ponteiro à função
    z = p(x,y); 
    printf("A soma dos numeros eh: %d",z);
    return 0
  }

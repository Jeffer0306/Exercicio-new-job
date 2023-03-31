#Execicio 01
#include <stdio.h>

int main() {
   int INDICE = 13, SOMA = 0, K = 0;

   while (K < INDICE) {
      K = K + 1;
      SOMA = SOMA + K;
   }

   printf("O valor da soma é: %d", SOMA);

   return 0;
} resposta será 91, pois usa um laço de repetição de loop while somando de 1 a 13, ele mantem na memoria todos os numeros que dá 91

#Exercicio 02

#include <stdio.h>

int main() {
   int num, a = 0, b = 1, c = 0;
   printf("Digite um número inteiro: ");
   scanf("%d", &num);

   while (c < num) {
      c = a + b;
      a = b;
      b = c;
   }

   if (c == num) {
      printf("%d pertence à sequência de Fibonacci.\n", num);
   } else {
      printf("%d não pertence à sequência de Fibonacci.\n", num);
   }

   return 0;
}

#Exercicio 03

a) A lógica é adicionar 2 a cada número. O próximo elemento é 9.

b) A lógica é multiplicar cada número por 2. O próximo elemento é 128.

c) A lógica é elevar o índice ao quadrado. O próximo elemento é 49 (7^2).

d) A lógica é adicionar 4 ao quadrado do índice. O próximo elemento é 100 (8^2 + 4).

e) A lógica é somar os dois números anteriores. O próximo elemento é 13 (5 + 8).

f) Não consigo realizar essa, talvez se considerar como numero primos para dar uma sequencia logica ai seria o 23, mas não posso afirmar.

#include <stdio.h>

int main() {
    float velocidade_carro = 110.0; // km/h
    float velocidade_caminhao = 80.0; // km/h
    float distancia = 100.0; // km
    float tempo_caminhao, distancia_carro;

    // Calcula o tempo que o caminhão leva para percorrer a distância
    tempo_caminhao = (distancia/2) / velocidade_caminhao + 5.0/60.0 + (distancia/2) / velocidade_caminhao + 5.0/60.0;

    // Calcula a distância percorrida pelo carro no mesmo tempo
    distancia_carro = velocidade_carro * tempo_caminhao;

    // Imprime o resultado
    printf("Distância percorrida pelo carro: %.1f km\n", distancia_carro);

    return 0;
}
#Exercicio 4
#include <stdio.h>

int main() {
    float velocidade_carro = 110.0; // km/h
    float velocidade_caminhao = 80.0; // km/h
    float distancia = 100.0; // km
    float tempo_caminhao, distancia_carro;

    // Calcula o tempo que o caminhão leva para percorrer a distância
    tempo_caminhao = (distancia/2) / velocidade_caminhao + 5.0/60.0 + (distancia/2) / velocidade_caminhao + 5.0/60.0;

    // Calcula a distância percorrida pelo carro no mesmo tempo
    distancia_carro = velocidade_carro * tempo_caminhao;

    // Imprime o resultado
    printf("Distância percorrida pelo carro: %.1f km\n", distancia_carro);

    return 0;
}
Só é necessario utilizar uma formula que considere, distância, velocidade e tempo de distancia percorrido por dois veiculos, nesse caso o caminhão estará mais perto de ribeirão quando se cruzr com o carro na rodavida.

# Exercicio 5

#include <stdio.h>
#include <string.h>

int main() {
    char string[100], invertida[100];
    int tamanho, i, j;
    
    printf("Digite uma string para ser invertida: ");
    scanf("%s", string);
    
    tamanho = strlen(string);
    
    for (i = tamanho - 1, j = 0; i >= 0; i--, j++) {
        invertida[j] = string[i];
    }
    
    invertida[j] = '\0';
    
    printf("A string invertida é: %s\n", invertida);
    
    return 0;
}
Todos os resultados estou apredendo agora na disciplina de desenvolvimento desktop que é em C, pois segunda minha professora, se você sabe C, você sabe todas as outras linguas.

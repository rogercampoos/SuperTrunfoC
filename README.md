# SuperTrunfoC , primeiro teste.

#include <stdio.h>

// Estrutura para armazenar os dados de uma carta do Super Trunfo
typedef struct {
    char estado;              // Uma letra de 'A' a 'H'
    char codigo[4];           // Exemplo: "A01" (3 caracteres + '\0')
    char cidade[50];          // Nome da cidade
    int populacao;            // Número de habitantes
    float area;               // Área em km²
    float PIB;                // PIB (em bilhões de reais)
    int pontosTuristicos;     // Número de pontos turísticos
} Carta;

int main(void) {
    Carta carta1, carta2;

    // Cadastro da Carta 1
    printf("Insira os dados da Carta 1:\n");
    
    printf("Estado (A a H): ");
    scanf(" %c", &carta1.estado);
    
    printf("Código da Carta (ex: A01): ");
    scanf("%s", carta1.codigo);
    
    // Lê o nome da cidade (permite espaços)
    printf("Nome da Cidade: ");
    scanf(" %[^\n]s", carta1.cidade);
    
    printf("População: ");
    scanf("%d", &carta1.populacao);
    
    printf("Área (em km²): ");
    scanf("%f", &carta1.area);
    
    printf("PIB (em bilhões de reais): ");
    scanf("%f", &carta1.PIB);
    
    printf("Número de Pontos Turísticos: ");
    scanf("%d", &carta1.pontosTuristicos);

    // Cadastro da Carta 2
    printf("\nInsira os dados da Carta 2:\n");
    
    printf("Estado (A a H): ");
    scanf(" %c", &carta2.estado);
    
    printf("Código da Carta (ex: B02): ");
    scanf("%s", carta2.codigo);
    
    printf("Nome da Cidade: ");
    scanf(" %[^\n]s", carta2.cidade);
    
    printf("População: ");
    scanf("%d", &carta2.populacao);
    
    printf("Área (em km²): ");
    scanf("%f", &carta2.area);
    
    printf("PIB (em bilhões de reais): ");
    scanf("%f", &carta2.PIB);
    
    printf("Número de Pontos Turísticos: ");
    scanf("%d", &carta2.pontosTuristicos);

    // Exibição dos dados cadastrados para cada carta
    printf("\nCarta 1:\n");
    printf("Estado: %c\n", carta1.estado);
    printf("Código: %s\n", carta1.codigo);
    printf("Nome da Cidade: %s\n", carta1.cidade);
    printf("População: %d\n", carta1.populacao);
    printf("Área: %.2f km²\n", carta1.area);
    printf("PIB: %.2f bilhões de reais\n", carta1.PIB);
    printf("Número de Pontos Turísticos: %d\n", carta1.pontosTuristicos);

    printf("\nCarta 2:\n");
    printf("Estado: %c\n", carta2.estado);
    printf("Código: %s\n", carta2.codigo);
    printf("Nome da Cidade: %s\n", carta2.cidade);
    printf("População: %d\n", carta2.populacao);
    printf("Área: %.2f km²\n", carta2.area);
    printf("PIB: %.2f bilhões de reais\n", carta2.PIB);
    printf("Número de Pontos Turísticos: %d\n", carta2.pontosTuristicos);

    return 0;
}

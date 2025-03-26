#include <cstdio>
#include <cstring>

int main() {
    char nome1[] = "Brasil", nome2[] = "Canadá";
    int populacao1 = 213000000, populacao2 = 38000000;
    float area1 = 8515767, area2 = 9984670;
    float pib1 = 2.05, pib2 = 1.84;
    int pontosTuristicos1 = 50, pontosTuristicos2 = 30;
    float densidade1 = 25.0, densidade2 = 3.8;
    
    int escolha;
    
    printf("Escolha um atributo para comparar:\n");
    printf("1 - Nome do país (não comparável)\n");
    printf("2 - População\n");
    printf("3 - Área\n");
    printf("4 - PIB\n");
    printf("5 - Número de pontos turísticos\n");
    printf("6 - Densidade demográfica\n");
    printf("Opção: ");
    scanf("%d", &escolha);
    
    printf("\nComparando %s e %s\n", nome1, nome2);
    
    switch (escolha) {
        case 1:
            printf("Nome dos países: %s vs %s\n", nome1, nome2);
            printf("Atributo não pode ser comparado. Escolha outro.\n");
            break;
        case 2:
            printf("População: %d vs %d\n", populacao1, populacao2);
            printf("Vencedor: %s\n", (populacao1 > populacao2 ? nome1 : nome2));
            break;
        case 3:
            printf("Área: %.2f km² vs %.2f km²\n", area1, area2);
            printf("Vencedor: %s\n", (area1 > area2 ? nome1 : nome2));
            break;
        case 4:
            printf("PIB: %.2f trilhões vs %.2f trilhões\n", pib1, pib2);
            printf("Vencedor: %s\n", (pib1 > pib2 ? nome1 : nome2));
            break;
        case 5:
            printf("Pontos turísticos: %d vs %d\n", pontosTuristicos1, pontosTuristicos2);
            printf("Vencedor: %s\n", (pontosTuristicos1 > pontosTuristicos2 ? nome1 : nome2));
            break;
        case 6:
            printf("Densidade demográfica: %.2f hab/km² vs %.2f hab/km²\n", densidade1, densidade2);
            printf("Vencedor: %s\n", (densidade1 < densidade2 ? nome1 : nome2));
            break;
        default:
            printf("Opção inválida!\n");
            break;
    }
    
    return 0;
}

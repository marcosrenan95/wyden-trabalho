#include <stdio.h>
#include <string.h>

struct Carta {
    char estado[50];
    char codigo[10];
    char cidade[50];
    int populacao;
    float area;
    float pib;
    int pontos_turisticos;
};

int main() {
    struct Carta parana, minas_gerais;

    // Dados do parana
    strcpy(parana.estado, "parana");
    strcpy(parana.codigo, "PR01");
    strcpy(parana.cidade, "curitiba");
    parana.populacao = 11800000;
    parana.area = 199.3;
    parana.pib = 614.61;
    parana.pontos_turisticos = 15;

    // Dados da minas gerais
    strcpy(minas_gerais.estado, "minas gerais");
    strcpy(minas_gerais.codigo, "MG01");
    strcpy(minas_gerais.cidade, "belo horizonte");
    minas_gerais.populacao = 20500000;
    minas_gerais.area = 586.5;
    minas_gerais.pib = 857.593;
    minas_gerais.pontos_turisticos = 49;

    // Comparação dos estados
    printf("Comparacao entre minas gerais e parana:\n\n");

    printf("Parana:\n");
    printf("  Populacao: %d\n", parana.populacao);
    printf("  Area: %.2f km²\n", parana.area);
    printf("  PIB: %.2f bilhoes\n", parana.pib);
    printf("  Pontos turisticos: %d\n\n", parana.pontos_turisticos);

    printf("Minas Gerais:\n");
    printf("  Populacao: %d\n", minas_gerais.populacao);
    printf("  Area: %.2f km²\n", minas_gerais.area);
    printf("  PIB: %.2f bilhoes\n", minas_gerais.pib);
    printf("  Pontos turisticos: %d\n\n", minas_gerais.pontos_turisticos);

    // Comparando população
    printf("Comparacao de populacao:\n");
    if (parana.populacao > minas_gerais.populacao) {
        printf("  Parana tem mais populacao que minas gerais.\n\n");
    } else if (minas_gerais.populacao > parana.populacao) {
        printf("  Minas gerais tem mais populacao que parana.\n\n");
    } else {
        printf("  Parana e minas gerais tem a mesma populacao.\n\n");
    }

    // Comparando área
    printf("Comparacao de area:\n");
    if (parana.area > minas_gerais.area) {
        printf("  Parana tem maior area que minas gerais.\n\n");
    } else if (minas_gerais.area > parana.area) {
        printf("  Minas gerais tem maior area que parana.\n\n");
    } else {
        printf("  Parana e minas gerais tem a mesma area.\n\n");
    }

    // Comparando PIB
    printf("Comparacao de PIB:\n");
    if (parana.pib > minas_gerais.pib) {
        printf("  Parana tem maior PIB que minas gerais.\n\n");
    } else if (minas_gerais.pib > parana.pib) {
        printf("  Minas gerais tem maior PIB que parana.\n\n");
    } else {
        printf("  Parana e minas gerais tem o mesmo PIB.\n\n");
    }

    // Comparando pontos turísticos
    printf("Comparacao de pontos turisticos:\n");
    if (parana.pontos_turisticos > minas_gerais.pontos_turisticos) {
        printf("  Parana tem mais pontos turisticos que minas gerais.\n\n");
    } else if (minas_gerais.pontos_turisticos > parana.pontos_turisticos) {
        printf("  Minas gerais tem mais pontos turisticos que parana.\n\n");
    } else {
        printf("  Parana e minas gerais tem o mesmo numero de pontos turisticos.\n\n");
    }

    return 0;
}

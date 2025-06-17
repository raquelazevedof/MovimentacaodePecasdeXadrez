#include <stdio.h>

// ------------------ TORRE ----------------------
// Função recursiva para movimentar a Torre 5 casas para a direita
void moverTorre(int casas) {
    if (casas == 0) return; // Caso base: quando não há mais casas para mover
    printf("Direita\n");     // Imprime a direção do movimento
    moverTorre(casas - 1);   // Chamada recursiva com uma casa a menos
}

// ------------------ BISPO (Recursivo) ----------------------
// Função recursiva para movimentar o Bispo 5 casas na diagonal "Cima Direita"
void moverBispoRecursivo(int casas) {
    if (casas == 0) return;
    printf("Cima Direita\n");
    moverBispoRecursivo(casas - 1);
}

// ------------------ BISPO (Loops Aninhados) ----------------------
// Função usando loops aninhados para simular o movimento do Bispo
void moverBispoComLoops(int casas) {
    // Loop externo representa o movimento vertical (Cima)
    for (int i = 0; i < casas; i++) {
        // Loop interno representa o movimento horizontal (Direita)
        for (int j = 0; j < 1; j++) { // Simula uma casa para a direita
            printf("Cima Direita\n");
        }
    }
}

// ------------------ RAINHA ----------------------
// Função recursiva para movimentar a Rainha 8 casas para a esquerda
void moverRainha(int casas) {
    if (casas == 0) return;
    printf("Esquerda\n");
    moverRainha(casas - 1);
}

// ------------------ CAVALO ----------------------
// Função para movimentar o Cavalo em L: 2 casas para cima e 1 para a direita
void moverCavalo() {
    int movimentos = 1; // Quantidade de movimentos em "L"
    
    // Loop externo para controlar a quantidade de "movimentos em L"
    for (int i = 0; i < movimentos; i++) {

        int subida = 0;

        // Loop while para subir duas casas
        while (subida < 2) {
            printf("Cima\n");
            subida++;
        }

        // Loop for para mover uma casa para a direita
        for (int j = 0; j < 1; j++) {
            if (j == 0) {
                printf("Direita\n"); // Movimento lateral do "L"
                continue; // Continua o loop, mesmo que ele só execute uma vez
            }
        }
    }
}

// ------------------ MAIN ----------------------
int main() {
    // ---------------- Torre ----------------
    printf("Movimento da Torre:\n");
    moverTorre(5); // Movimenta a torre 5 casas para a direita
    printf("\n");

    // ---------------- Bispo (Recursivo) ----------------
    printf("Movimento do Bispo (Recursivo):\n");
    moverBispoRecursivo(5); // Movimenta o bispo 5 casas em diagonal com recursão
    printf("\n");

    // ---------------- Bispo (Loops Aninhados) ----------------
    printf("Movimento do Bispo (Loops Aninhados):\n");
    moverBispoComLoops(5); // Movimenta o bispo com loops aninhados
    printf("\n");

    // ---------------- Rainha ----------------
    printf("Movimento da Rainha:\n");
    moverRainha(8); // Movimenta a rainha 8 casas para a esquerda
    printf("\n");

    // ---------------- Cavalo ----------------
    printf("Movimento do Cavalo:\n");
    moverCavalo(); // Movimenta o cavalo em L (2 cima, 1 direita)

    return 0;
}
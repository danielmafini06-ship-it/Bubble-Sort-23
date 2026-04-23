#include <stdio.h>

int main() {
    int v[] = {5, 2, 9, 1, 5};
    int tam = 5;
    int aux;
    for (int i = 0; i < tam - 1; i++) {
        for (int j = 0; j < tam - i - 1; j++) {
            if (v[j] > v[j + 1]) {
                aux = v[j];
                v[j] = v[j + 1];
                v[j + 1] = aux;
 } } }
    for (int i = 0; i < tam; i++) printf("%d ", v[i]);
}